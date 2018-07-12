pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Dit Bonjour') {
      steps {
        echo "Bonjour ${MY_NAME}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'D1@N3'
  }
}