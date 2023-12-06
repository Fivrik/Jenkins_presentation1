pipeline {
  agent any
  stages {
    stage('Load Groovy File') {
      steps {
        load 'pipeline.groovy'
      }
    }

    stage('Test') {
      steps {
        echo 'This is the Test stage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'This is the Deploy stage'
      }
    }

  }
}