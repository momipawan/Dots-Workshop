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
        timeout(time: 10, unit: 'MINUTES')
      }
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
      }
    }
  }
}