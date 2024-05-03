pipeline {
    agent any
    environment {
        SCANNER_HOME = tool 'sonar-scanner'
    }

    stages {
        stage('Checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/DevyanshSamyal/automated-pipeline-for-course-material.git'
            }
        }

        stage('Installing packages') {
            steps {
                script {
                  
                    
                    // Install required python packages within the virtual environment
                    sh 'pip install -r requirements.txt'
                }
            }
        }


       
    }
}
