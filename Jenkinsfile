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
                bat "javac App.java java App"
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
