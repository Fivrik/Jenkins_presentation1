pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is the Build stage'
        load 'pipeline.groovy'
        archiveArtifacts(artifacts: 'function', allowEmptyArchive: true)
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