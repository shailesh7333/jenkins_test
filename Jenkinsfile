pipeline {
  agent any
  stages {
    stage('Echo') {
      parallel {
        stage('Echo') {
          steps {
            echo 'Hello World'
          }
        }

        stage('Echo2') {
          steps {
            echo 'Hello World 2'
          }
        }

      }
    }

  }
}