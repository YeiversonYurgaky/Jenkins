pipeline {
    agent any
    stages {
        stage ('Test app') {
            steps {
                // Run Maven tests
                bat 'mvn clean test'
            }
        }
        stage('Check coverage') {
            steps {
                script {
                    bat 'mvn jacoco:check'
                }
            }
        }
    }
}
