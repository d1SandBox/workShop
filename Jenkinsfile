pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Dit Bonjour') {
      steps {
        echo "Bonjour ${MY_NAME}"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'D1@N3'
    TEST_USER = credentials('test-user')
  }
}