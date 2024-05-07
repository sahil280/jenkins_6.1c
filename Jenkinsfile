pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add build-related commands here, or replace with actual commands later
            }
            post {
                success {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Build Stage Successful: ${currentBuild.fullDisplayName}",
                         body: "The build stage completed successfully. Check Jenkins for more details."
                }
                failure {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Build Stage Failed: ${currentBuild.fullDisplayName}",
                         body: "The build stage failed. Check Jenkins for more details."
                }
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests...'
                // Add test-related commands here, or replace with actual commands later
            }
            post {
                success {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Test Stage Successful: ${currentBuild.fullDisplayName}",
                         body: "The test stage completed successfully. Check Jenkins for more details."
                }
                failure {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Test Stage Failed: ${currentBuild.fullDisplayName}",
                         body: "The test stage failed. Check Jenkins for more details."
                }
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analyzing code...'
                // Add code analysis commands here, or replace with actual commands later
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Performing security scan...'
                // Add security scan commands here, or replace with actual commands later
            }
            post {
                success {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Security Scan Stage Successful: ${currentBuild.fullDisplayName}",
                         body: "The security scan stage completed successfully. Check Jenkins for more details."
                }
                failure {
                    mail to: 'jasolliyasahil2@gmail.com',
                         subject: "Security Scan Stage Failed: ${currentBuild.fullDisplayName}",
                         body: "The security scan stage failed. Check Jenkins for more details."
                }
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging...'
                // Add deployment commands for staging here, or replace with actual commands later
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging...'
                // Add integration tests on staging commands here, or replace with actual commands later
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production...'
                // Add deployment commands for production here, or replace with actual commands later
            }
        }
    }
}
