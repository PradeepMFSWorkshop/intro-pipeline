pipeline {
  agent {
    label 'jdk10'
  }
  stages {
    stage('Hello') {
      steps {
        echo "Hello ${params.Name}"
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
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}