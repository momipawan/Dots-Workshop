pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'hello'
      }
    }
    stage('Deploy') {
      options {
        timeout(time: 10, unit: 'SECONDS')
      }
      steps {
        echo 'Continuing with deployment'
      }
    }
  }
}