@Library('libpipelines@master') _

hose {
    EMAIL = 'front'
    MODULE = 'egeo-ui-fonts'
    DEVTIMEOUT = 30
    RELEASETIMEOUT = 30
    REPOSITORY = 'egeo-ui-fonts'

    DEV = { config ->
        doCompile(config)
        doDeploy(config)

    }
}
