pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
          args '-u 0'
        }

      }
      steps {
        sh '''id
env
pwd'''
        sh 'apt update'
        sh 'apt -y install gcc make libpcap-dev'
        sh './configure'
      }
    }
  }
}