pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Demo Application'
        sh ' sh \'mvn -Dversion=3 compile\' '
      }
    }

  }
}