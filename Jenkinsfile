pipeline {
    agent any

    stages {
        stage('git') {
            steps {
               git branch: 'main', url: 'https://github.com/En4128/dockerjenkins.git'
            }
        }
        stage('dockerbuild'){
            steps{
                sh '''docker build -t img2 .
                       docker run img2'''
            }
            
        }
    }
}
