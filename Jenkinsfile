pipeline {
    agent any

    stages {
        stage("Docker pull") {
            steps {
                sh 'docker pull librecores/librecores-ci-openrisc'
                sh 'docker images'
            }
        }

       stage("Yosys synthesis"){
            steps {
               sh 'docker run --rm -v $(pwd):/src -w /src nancy-nano /bin/bash -c \
               "fusesoc library add mor1kx /src; \
                fusesoc run --target=synth mor1kx; \
                /test-scripts/extract-yosys-stats.py < build/mor1kx_*/synth-icestorm/yosys.log"'
            }
        }

        stage('Generate Resource Usage Report') {
            steps {
                echo "-=- report metrics -=-"
                plot csvFileName: 'plot-yosys-stats.csv', csvSeries: [
                    [
                        file: 'yosys-stats.csv',
                        url: ''
                    ]
                ], exclZero: true,
                group: 'Resource Usage',
                numBuilds: '15',
                style: 'line',
                title: 'Resource Usage',
                useDescr: true,
                yaxis: 'Values'

                echo "-=- report metrics -=-"

            }
        }
    }
}
