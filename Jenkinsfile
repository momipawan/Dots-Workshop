pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'hello'
      }
    }
    stage('Deploy') {
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
      }
    }
  }
}