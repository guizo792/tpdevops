pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'cd tpdevops;mvn clean'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'cd tpdevops;mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'cd tpdevops;mvn package'
            }
        }
    }
}
