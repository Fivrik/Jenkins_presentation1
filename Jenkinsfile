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
            sh '''def pipeline = load
\'pipeline.groovy\'
pipeline.functionA()
pipeline.functionB()'''
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