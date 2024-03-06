pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file using a shell script
                sh 'g++ -o PES1UG21CS343-1 main.cpp'
            }
        }
        stage('Test') {
            steps {
                // Print output of the compiled .cpp file
                sh './PES1UG21CS343-1'
            }
        }
        stage('Deploy') {
            steps {
                // Deployment steps if needed
                // This stage is empty in this example
            }
        }
    }
    
    post {
        always {
            // Display 'pipeline failed' in case of any errors
            echo 'Pipeline failed'
        }
    }
}
