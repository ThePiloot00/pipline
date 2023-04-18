pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'git clone https://github.com/ThePiloot00/pipline.git'
		echo 'ripo clond'
		sh 'cd pipline'
		sh './gradlew bootRun > /dev/null 2>&1 &'
		echo 'start app'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
