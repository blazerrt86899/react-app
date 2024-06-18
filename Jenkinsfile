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
        nodejs('node-10.17') {
          sh 'yarn install'
          sh 'yarn build'
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
