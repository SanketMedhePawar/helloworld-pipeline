pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/SanketMedhePawar/helloworld-pipeline.git'
            }
        }
        stage('Run Script') {
            steps {
                echo 'I am in Run Script stage'
                sh 'git --version'
                sh 'docker --version'
                sh 'mvn -v'
            }
        }
    }
}
