pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Execute build commands here
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Execute test commands here
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Execute deployment commands here
                sh './main.sh'
		sh 'echo "Deployed"'
            }
        }
    }
}
