pipeline {
  agent {
    node {
      label 'worker_node1'
    }

  }
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/ghXplorer/ansible-playbook.git'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Build done!'
  }
}