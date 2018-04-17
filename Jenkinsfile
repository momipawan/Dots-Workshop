pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo "Hello ${MY_NAME}"
        echo "Hello ${params.Name}!"
      }
    }
  }
  environment {
    MY_NAME = 'Pawan'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}