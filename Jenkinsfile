pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build in process'
      }
    }
    stage('Test firefox') {
      parallel {
        stage('Test firefox') {
          steps {
            sh 'echo \'testing Firefox\''
          }
        }
        stage('Test Chrome') {
          steps {
            sh 'echo \'testing Chrome\''
          }
        }
        stage('Test edge') {
          steps {
            sh 'echo \'Testing edge\''
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }
  }
}