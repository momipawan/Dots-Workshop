pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'hello'
      }
    }
  }
  post {
    aborted {
      echo 'Why didn\'t you push my button?'
      
    }
    
  }
}