pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Building the code using Maven to compile and package the application.'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Running unit tests with JUnit and integration tests with Selenium.'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Analysing code quality using SonarQube to ensure industry standards are met.'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Performing security scan using OWASP Dependency-Check to identify vulnerabilities.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploying application to staging server on AWS EC2 instance.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Running integration tests on staging environment to verify production-like behaviour.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploying application to production server on AWS EC2 instance.'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
