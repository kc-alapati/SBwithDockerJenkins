pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            git'https://github.com/kc-alapati/SBwithDockerJenkins.git'
            sh './mvnw compile'
                echo 'Maven build successs'
            }
        }
        stage('Test') {
            steps {
            sh './mvnw test'
                echo 'Test cases execution successs'
            }
        }
        stage('Deploy') {
            steps {
            sh './mvnw package'
                echo 'Application deployment successs'
            }
        }
    }
}