pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/SanketMedhePawar/helloworld-pipeline.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    dockerImage = docker.build("helloworld-image")
                    sh 'Docker Image build successfull'
                }
            }
        }

        stage('Run in Docker') {
            steps {
                script {
                    dockerImage.run()
                    sh 'Container created'
                }
            }
        }
    }
}
