pipeline {
  agent any
  stages {
    stage('Dit Bonjour') {
      steps {
        echo 'Bonjour Le Monde'
      }
    }
    stage('Java Version') {
      steps {
        sh 'java -version'
        bat 'java -version'
      }
    }
  }
}