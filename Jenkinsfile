pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is the Build stage'
        archiveArtifacts(artifacts: '**/git', allowEmptyArchive: true)
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