pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Dit Bonjour') {
      parallel {
        stage('Dit Bonjour') {
          steps {
            echo "Hello ${params.Name}!"
            sh 'java -version'
            echo "Username: ${TEST_USER_USR}"
            echo "Password: ${TEST_USER_PSW}"
          }
        }
  stage('Deploy') {
      options {
        timeout(time: 30, unit: 'SECONDS') 
      }
     input {
        message "Which Version?"
        ok "Deploy"
        parameters {
            choice(name: 'APP_VERSION', choices: "v1.1\nv1.2\nv1.3", description: 'What to deploy?')
        }
      }
      steps {
        echo "Deploying ${APP_VERSION}."
      }
    }
      }
    }
  }
  environment {
    MY_NAME = 'D1@N3'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: "${MY_NAME}, description: 'Who should I say hi to?')
  }
}
