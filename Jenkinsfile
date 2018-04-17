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
        message 'Which Version?'
        id 'Deploy'
        parameters {
          choice(name: 'APP_VERSION', choices: '''v1.1
v1.2
v1.3''', description: 'What to deploy?')
        }
      }
      steps {
        echo "Deploying ${APP_VERSION}."
      }
    }
  }
}