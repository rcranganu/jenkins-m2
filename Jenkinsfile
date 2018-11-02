node {
    //Clean workspace before doing anything
    deleteDir()

    try {
        stage ('Clone') {
            checkout scm
        }
    } catch (err) {
        currentBuild.result = 'Failed'
        throw err
    }
}
