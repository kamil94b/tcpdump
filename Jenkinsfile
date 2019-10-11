pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
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