pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ jenk.cpp -o jenk'
      }
    }
    
    stage('Test') {
      steps {
        sh './jenk'
      }
    }
    
    stage('Deploy') {
      steps {
        echo 'BROKE'
      }
    }
  }
  
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
