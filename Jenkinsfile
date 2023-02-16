pipeline {
  agent any

  stages {
 
 
    stage('build') {
      steps {
        sh 'g++ jenk.cpp -o jenk'
      }
    }

   
    stage('test') {
      steps {
        sh './jenk'
      }
    }
   

    stage('deploy') {
      steps {
      }
    }
  
 
 
  post {
    failure {
      echo 'pipeline isn1t successful'
    }
  }
}
