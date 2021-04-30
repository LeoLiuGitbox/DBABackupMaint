pipeline {
  agent none
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout from GetHub'
        git 'https://github.com/LeoLiuGitbox/DBABackupMaint.git'
      }
    }

    stage('Build') {
      steps {
        powershell './get-logins.ps1'
      }
    }

  }
}
