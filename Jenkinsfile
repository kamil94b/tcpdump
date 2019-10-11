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
        sh 'id'
        sh 'apk add gcc'
        sh './configure'
      }
    }
  }
}