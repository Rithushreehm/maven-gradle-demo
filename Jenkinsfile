pipeline {
    agent any

    stages {

        stage('Maven Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Maven Package') {
            steps {
                bat 'mvn package'
            }
        }

        stage('Gradle Build') {
            steps {
                bat 'gradle build'
            }
        }

        stage('Gradle Test') {
            steps {
                bat 'gradle test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Application Deployed Successfully'
            }
        }
    }
}
