pipeline {
    agent any
    stages {
        stage('build') {
            agent {
                docker {
                    image 'maven:3.8.4-openjdk-11-slim'
                    reuseNode true
                }
            }
            steps {
                sh 'mvn --version'
            }
        }
    }
}
