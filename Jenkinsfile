pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES2UG20CS147-1 josmin.cpp'
        echo 'Build Stage Successful
      }
    }
    stage('Test') {
      steps {
        sh './PES2UG20CS147-1'
        echo 'Test Stage Successful'
        }
    }
    stage('Deploy') {
      steps {
        echo 'Deployment Successful
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
