pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Demo Application'
        sh 'sh `mvn  compile` '
      }
    }

    stage('Test') {
      steps {
        echo 'Test Step'
        sh 'sh `mvn  test` '
      }
    }

    stage('Deliver') {
      steps {
        echo 'Deliver'
        sh 'sh `./jenkins/scripts/deliver.sh` '
      }
    }

  }
}