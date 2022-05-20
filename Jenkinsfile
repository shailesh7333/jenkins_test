pipeline {
  agent any
  stages {
    stage('Log Tool Version') {
      parallel {
        stage('Log Tool Version') {
          steps {
            sh '''mvn --version
git --version
java --version'''
          }
        }

        stage('Check pom.xml file') {
          steps {
            fileExists 'pom.xml'
          }
        }

      }
    }

    stage('Post Build Steps') {
      steps {
        writeFile(file: 'completed.txt', text: 'It worked!')
      }
    }

  }
}