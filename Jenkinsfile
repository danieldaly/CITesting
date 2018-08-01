pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './gradlew assembleDebug'
      }
    }
    stage('Test') {
      agent any
      steps {
        sh './gradlew testDebugUnitTest'
      }
    }
  }
}