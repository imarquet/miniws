pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello'
        echo 'On build !'
      }
    }
    stage('Deploy to QA') {
      parallel {
        stage('Deploy to QA') {
          steps {
            sleep 5
            echo 'On dÃ©ploie en Recette'
          }
        }
        stage('qualit�') {
          steps {
            echo 'on check la qualit�'
          }
        }
      }
    }
    stage('Tests') {
      steps {
        echo 'On teste'
        sleep 5
      }
    }
    stage('Deploy to prod') {
      steps {
        input(message: 'on deploie ??', ok: 'GO !!')
        echo 'go deploy prod'
      }
    }
  }
}