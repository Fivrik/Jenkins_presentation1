pipeline {
  agent any
  stages {
    stage('Load Groovy File') {
      steps {
        script {
          def pipeline = load 'pipeline.groovy'
          pipeline.functionA()
          pipeline.functionB()
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
