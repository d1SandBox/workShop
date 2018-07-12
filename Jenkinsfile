pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Dit Bonjour') {
      steps {
        echo "Bonjour ${MY_NAME}"
        sh 'java -version'
        echo "Username: ${TEST_USER_USR}"
        echo "Password: ${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'D1@N3'
    TEST_USER = credentials('test-user')
  }
}