pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
               'https://github.com/SanketMedhePawar/helloworld-pipeline.git'
            }
        }

        stage('Run Script') {
            steps {
                sh 'python3 helloworld.py'
            }
        }
    }
}
