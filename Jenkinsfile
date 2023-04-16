pipeline {
    agent any

    stages {

        stages ('Build Docker Image') {
            steps {
                scripts {
                    dockerapp = docker.build ("fabrinascimento/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }
}