pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Dit Bonjour') {
      steps {
        echo 'Bonjour Le Monde'
      }
    }
    stage('Java Version') {
      steps {
        sh 'java -version'
      }
    }
  }
}