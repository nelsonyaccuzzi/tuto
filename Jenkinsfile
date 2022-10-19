pipeline {
    agent { label 'tuto' }
    

    stages {
        stage('Build') {
            steps {
                container('podman') {
                    script {
                        sh 'podman ps'
                    }
                }
                container('kubectl') {
                    script {
                        sh 'kubectl version'
                    }
                }
            }
        }
    }
}
