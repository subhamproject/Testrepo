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
          ssh -l ec2-user 52.66.77.108
          '''
        }
      }
    }
  }
}
