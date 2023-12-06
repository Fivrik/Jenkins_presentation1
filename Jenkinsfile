pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is the Build stage'
            load 'pipeline.groovy'
            archiveArtifacts(artifacts: 'function', allowEmptyArchive: true)
          }
        }

        stage('Load Groovy File') {
          steps {
            load 'pipeline.groovy'
          }
        }

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