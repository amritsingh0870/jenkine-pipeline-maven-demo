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
                bat "java App"
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
