pipeline {
  agent any
  stages {
    stage('Clone') {
      parallel {
        stage('Clone') {
          agent any
          steps {
            echo 'clone code'
            sleep 1
          }
        }

        stage('Email') {
          steps {
            emailext(subject: 'send email', body: 'hello', to: 'fimtestuvw@gmail.com')
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'testing'
      }
    }

    stage('Report') {
      steps {
        echo 'report'
      }
    }

  }
}