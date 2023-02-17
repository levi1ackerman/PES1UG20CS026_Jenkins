pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ cclab.cpp'
                echo "Build Successful!"
            }
        }
      stage('Test') {
        steps {
          sh './a.out'
          echo "Test Successful!"
        }
      }
      stage('Deploy') {
          steps {
        echo "Deploy"
          }
      }
    }
    post {
        failure {
            echo "Pipeline failed!"
        }
    }
}
