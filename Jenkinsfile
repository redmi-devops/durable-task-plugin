def builds = [:]
builds['docker'] = { buildPlugin(platforms: ['docker']) }
builds['docker'] = {
    withEnv(['SKIP_DURABLE_TASK_BINARY_GENERATION=true']) {
        buildPlugin(platforms: ['docker'])
    }
}
parallel builds
