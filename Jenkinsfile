pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh './gradlew compile release Sources'
      }
    }

  }
  environment {
    APP_NAME = 'test'
  }
}