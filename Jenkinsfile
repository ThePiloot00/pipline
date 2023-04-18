pipeline {
    agent{ docker { image 'gradle:8.1.0-jdk17' } }

    stages {
        stage('Build') {
            steps {
                sh 'git clone https://github.com/ThePiloot00/pipline.git'
		echo 'ripo clond'
		sh 'cd pipline'
		sh './gradlew bootRun'
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
