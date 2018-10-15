pipeline {
  agent {
    label 'jdk10'
  }
  stages {
    stage('Hello') {
      steps {
        echo "$My_Name"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    My_Name = 'Pradeep'
    TEST_USER = credentials('test-user')
  }
}