pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is the Build stage'
        archiveArtifacts(artifacts: '\'**/*.html\'', allowEmptyArchive: true)
      }
    }

    stage('Test') {
      steps {
        echo 'This is the Test stage'
        archiveArtifacts(artifacts: '\'**/*.html\'', allowEmptyArchive: true)
      }
    }

    stage('Deploy') {
      steps {
        echo 'This is the Deploy stage'
        archiveArtifacts(artifacts: '\'**/*.html\'', allowEmptyArchive: true)
      }
    }

  }
}