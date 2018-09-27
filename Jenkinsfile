pipeline {
    agent any

    stages {
        stage('CLEAN') {
            steps {
                echo 'Cleaning..'
                sh "mvn clean"
            }
        }
        stage('TEST') {
            steps {
                echo 'Testing..'
                sh "mvn test"
            }
        }
        stage('PACKAGE') {
            steps {
                echo 'Deploying....'
                sh "mvn package"
            }
        }
    }
}
