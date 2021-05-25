#!groovy
pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                bat '.\gradlew build'
            }
            post {
                always {
                    junit '**/build/test-results/integrationTest/TEST-*.xml'
                    }
            }
        }
        stage('Test'){
            steps {
                echo "integration tests"
            }
            post {
                always {
                    junit '**/build/test-results/integrationTest/TEST-*.xml'
                    }
            }
        }
        stage('Deploy') {
            steps {
                gradle run
            }
        }
    }
}