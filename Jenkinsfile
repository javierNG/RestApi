pipeline {
    agent any

    triggers {
            pollSCM('* * * * *')
    }

    environment {
        DOCKER_USERNAME = 'sivaprasadreddy'
        APPLICATION_NAME = 'RESTApi'
    }

    parameters {
        booleanParam(name: 'PUBLISH_TO_DOCKERHUB', defaultValue: false, description: 'Publish Docker Image to DockerHub?')
    }

    stages {
        stage('Build'){
            steps{
                echo 'Building'
            }
        }
        stage('Test'){
            steps{
                echo 'testing'
            }
        }
        stage('Deploy it') {
            steps{
                echo 'deploying the app'
            }
        }
    }
}