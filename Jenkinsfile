pipeline {
  agent any
  stages {
    stage('Build') {
      environment {
        Dev = '1'
      }
      steps {
        echo 'Here be the start'
        sleep 5
        echo 'Here be the end of build'
      }
    }
  }
}