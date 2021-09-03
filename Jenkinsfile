pipeline {
    agent any

    stages {
        stage('Design') {
            steps {
                echo 'Design Hello World'
            }
        }
        stage('Build') {
            steps {
                echo 'Building Hello World'
                sleep 2
            }
        }
        stage('Testing') {
            steps {
                echo 'Testing Hello World'
                sleep 1
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Hello World'
            }
        }
        stage('Test') {
            steps {
                echo 'preProdTesting Hello World'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing Hello World'
                sleep 1
                git branch: 'main', credentialsId: 'myGitCredentials', url: 'https://github.com/alexvolk001/JenkinsDemo.git'
            }
        }
    }
}
