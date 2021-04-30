pipeline {
  agent none
  stages {
      stage('Get Repository') {
      agent {
        node {
          label 'master'
        }

    stage('Checkout') {
      steps {
        echo 'Checkout from GetHub'
        Checkout scm
      }
    }

    stage('Build') {
      steps {
        powershell 'Get-Service'
        powershell '''
                    ./scripts/get-logins.ps1
        ''' 
      }
    }

  }
}
