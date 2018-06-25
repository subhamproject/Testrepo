#!groovy

pipeline {
  options {
    buildDiscarder(logRotator(numToKeepStr: '10'))
  }
  agent any
  stages {
    stage('Deployment') {
      steps {
        script {
          sh '''
          ssh -l pentaho 52.66.77.108
          '''
        }
      }
    }
  }
}
