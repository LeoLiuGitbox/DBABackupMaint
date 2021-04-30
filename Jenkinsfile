pipeline {
  
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout from GetHub'
        git 'https://github.com/LeoLiuGitbox/DBABackupMaint.git'
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
