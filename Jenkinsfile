pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh './gradlew compile release Sources'
      }
    }

    stage('build') {
      steps {
        sh '''./gradlew assemble release
./gradlew generatePomFileForLibraryPublication'''
      }
    }

  }
  environment {
    APP_NAME = 'test'
  }
}