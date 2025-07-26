pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
               'https://github.com/SanketMedhePawar/helloworld-pipeline.git', branch: 'main'
            }
        }

        stage('Run Script') {
            steps {
                sh 'python3 helloworld.py'
            }
        }
    }
}
