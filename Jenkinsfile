pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        sh '''id
env
pwd'''
        sh 'sudo apk add gcc'
        sh './configure'
      }
    }
  }
}