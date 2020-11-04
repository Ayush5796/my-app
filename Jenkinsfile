pipeline {
    agent any 
    stages {
        stage('Clone Repo and Clean It') { 
            steps {
                bat "mvn clean "
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test" 
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package" 
            }
        }
    }
}
