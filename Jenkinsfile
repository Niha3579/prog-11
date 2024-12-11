pipeline {
    agent any 
    stages{
        stage('Build'){
            steps {
                script {
                    echo "building"
                    bat "docker build -t new:latest ."
                    bat "docker run -d new:latest"
                }
            }
        }
         stage('run'){
            steps {
                script {
                    echo "runnig"
                }
            }
        }
         stage('testing'){
            steps {
                script {
                    echo "testing"
                }
            }
        }
    }
}