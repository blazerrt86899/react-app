pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Building the application...."
        script {
          def test = 2 + 2 > 3 ? 'Cool':'Not Cool'
          echo test
        }
      }
    }
    stage('Test') {
      steps {
        echo "Testing the application...."
      }
    }
    stage('Deploy') {
      steps {
        echo "Deploying the application...."
      }
    }
  }
}
