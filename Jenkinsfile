pipeline {
  agent {
    label 'jdk10'
  }
  stages {
    stage('Hello') {
      steps {
        echo "$My_Name"
        sh 'java -version'
      }
    }
  }
  environment {
    My_Name = 'Pradeep'
  }
}