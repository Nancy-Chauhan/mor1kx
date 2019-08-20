@Library('lcci') _

openrisc_ci ([
        [name: 'verilator', job: 'verilator' ],
        [
                name: 'Testing-1',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy"
        ],
        [
                name: 'Testing-2',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs: "--feature_dmmu NONE"
        ],
        [
                name: 'Testing-3',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-dsxinsn",
                extraCoreArgs: "--feature_immu NONE"
        ],
        [
                name: 'Testing-4',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_datacache NONE"
        ],
        [
                name: 'Testing-5',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_instructioncache NONE"
        ],
        [
                name: 'Testing-6',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_debugunit NONE"
        ],
        [
                name: 'Testing-7',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-cmov",
                extraCoreArgs:"--feature_cmov NONE"
        ],
        [
                name: 'Testing-8',
                job: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-ext",
                extraCoreArgs:"--feature_ext NONE"
        ]
])
