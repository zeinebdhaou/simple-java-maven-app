pipeline {
  agent any
  stages {
    stage('Build ') {
      steps {
        echo ' Build Demo Application'
        sh 'mvn  compile'
      }
    }

    stage('Test') {
      steps {
        echo 'Test Demo Application'
        sh ' test '
      }
    }

    stage('Deliver') {
      steps {
        echo 'Deliver Demo Application'
        sh './jenkins/scripts/deliver.sh'
      }
    }

  }
}