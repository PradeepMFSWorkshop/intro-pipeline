pipeline {
  agent {
    label 'jdk10'
  }
  stages {
    stage('Hello') {
      steps {
        echo 'Hello World'
        sh 'java -version'
      }
    }
  }
}