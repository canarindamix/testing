pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
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
        stage('Parallel stuff') {
          steps {
            echo 'Sending email'
            emailext(subject: 'What a beautiful day', body: 'We are gonna be great', attachLog: true, from: 'agentX', to: 'aurelien.chauvey@ericsson.com')
            echo 'Email sent'
          }
        }
      }
    }
  }
}