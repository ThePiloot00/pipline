pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
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
