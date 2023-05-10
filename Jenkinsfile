pipeline {
  agent any
  stages {
    stage('Pull') {
      checkout scm
    }

    stage('build') {
      steps {
        sh 'echo "hello ini pipeline"'
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}