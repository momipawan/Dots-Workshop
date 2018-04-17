pipeline {
  agent {
    docker {
      image 'golang:1.10.1-alpine'
    }
    
  }
  stages {
    stage('Hello') {
      steps {
        echo 'Hello-world'
      }
    }
  }
}