node {
    //Clean workspace before doing anything
    deleteDir()

    try {
        stage ('Clone') {
            checkout scm
        }
        stage ('Install') {
            sh 'composer install'
        }
    } catch (err) {
        currentBuild.result = 'Failed'
        throw err
    }
}
