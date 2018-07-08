pipeline {
  agent any
  stages {
    stage('Ansible') {
      steps {
        sh 'cp -rf ansible/* /etc/ansible'
      }
    }
  }
}