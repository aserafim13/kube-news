pipeline {
    agent any

    stages {

        stage ('Build docker image') {
            steps {
                script {
                    dockerapp = docker.build ("aserafim/kube-news:${env.BUILD.ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}
