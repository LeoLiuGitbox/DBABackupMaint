pipeline { 
  agent any
  stages {      
    stage('Checkout') {
      steps {
        echo 'Checkout from GetHub'
        checkout scm
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
