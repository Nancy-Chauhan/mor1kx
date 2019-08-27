openriscPipeline {

    yosysReport {
		core 'mor1kx'
		target 'synth'
		logPath 'build/mor1kx_*/synth-icestorm/yosys.log'
	}

    job('verilator') {
        job 'verilator'
    }

    job('icarus-cappuccino') {
        job 'or1k-tests'
        sim 'icarus'
        pipeline 'CAPPUCCINO'
        expectedFailures 'or1k-cy'
    }
}
