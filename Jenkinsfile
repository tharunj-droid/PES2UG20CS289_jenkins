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
        echo '/DEPART/services'
      }
    }
  }
  
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
