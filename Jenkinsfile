pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo "Name ${params.Name}!"
      }
    }
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}