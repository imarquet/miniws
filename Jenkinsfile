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
      steps {
        sleep 5
        echo 'On déploie en Recette'
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
        echo 'On deploie en prod'
        sleep 5
      }
    }
  }
}