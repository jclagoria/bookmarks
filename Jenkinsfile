pipeline {
  agent {
    node {
      label 'test'
    }

  }
  stages {
    stage('stage-1') {
      parallel {
        stage('stage-1') {
          steps {
            readMavenPom(file: 'pom.xml')
          }
        }
        stage('stage-1-b') {
          steps {
            echo 'hello'
          }
        }
      }
    }
  }
}