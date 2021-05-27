#!groovy

pipeline {
    agent any

    tools {
        maven "maven"
    }

    stages {
        stage("Build") {
            steps {
                bat "mvn -version"
                bat "mvn clean"
            
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
