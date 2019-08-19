@Library('lcci') _

openrisc_ci ([
        [name: 'verilator'],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs: "--feature_dmmu NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-dsxinsn",
                extraCoreArgs: "--feature_immu NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_datacache NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_instructioncache NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy",
                extraCoreArgs:"--feature_debugunit NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-cmov",
                extraCoreArgs:"--feature_cmov NONE"
        ],
        [
                name: 'or1k-tests',
                sim: 'icarus',
                pipeline: 'CAPPUCCINO',
                expectedFailures: "or1k-cy or1k-ext",
                extraCoreArgs:"--feature_ext NONE"
        ]
])
