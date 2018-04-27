pipeline {
  agent any
  stages {
    stage('CheckOut') {
      steps {
        echo 'Checkout is completed'
      }
    }
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build Is running'
            timeout(time: 2200, unit: "SECONDS")
          }
        }
        stage('Unit-Test') {
          steps {
            echo 'Unit Testing is completed'
          }
        }
        stage('Regression Test') {
          steps {
            echo 'Regression Testing is completed'
          }
        }
        stage('Integration Test') {
          steps {
            echo 'Integration Tetsing is completed'
          }
        }
      }
    }
    stage('Upload To Nexus') {
      steps {
        echo 'Artifacts is uploading to Nexus'
      }
    }
  }
}
