pipeline {
  agent any
  stages {
    stage('Pull') {
      steps {
        git(credentialsId: 'samsul-ssh-project', url: 'git@github.com:samsuldemo/samsul-flask-demo.git', branch: 'main')
      }
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