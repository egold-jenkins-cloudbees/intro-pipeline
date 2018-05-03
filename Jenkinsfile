pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        echo 'Hello World!?'
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
  environment {
    TEST_USER = credentials('test-user')
    MY_NAME = 'Gold-ENV'
  }
}