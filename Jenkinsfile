pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        parallel(
          "Test": {
            sh 'echo "Testing..."'
            
          },
          "Unittests": {
            sh 'echo "Unittests"'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploying..."'
      }
    }
  }
}