pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/ghXplorer/ansible-playbook.git'
      }
    }

    stage('Build') {
      steps {
        tool 'gradle4'
        sh 'gradle build'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Build done!'
  }
}