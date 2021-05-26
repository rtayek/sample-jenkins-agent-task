pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                bat 'gradlew.bat clean build'
            }
        }
    }
}

