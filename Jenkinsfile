pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ raj.cpp -o raj'
        echo 'compiled to binary'
      }
    }
    
    stage('Test') {
      steps {
        sh './raj'
      }
    }
    
    stage('Deploy') {
      steps {
        echo 'done!'
        sh 'i am not working'
      }
    }
  }
  
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
