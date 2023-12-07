pipeline {
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage('Build Maven'){
            steps{
                git changelog: false, poll: false, url: 'https://github.com/prabhuitz7120/docker.git'
                sh 'mvn clean install'
            }
        }
    }
}
