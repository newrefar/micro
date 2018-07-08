pipeline {
  agent any
  stages {
    stage('Move') {
      steps {
        sh '''mkdir /var/jenkins_home/micro

cp -rf * /var/jenkins_home/micro'''
      }
    }
  }
}