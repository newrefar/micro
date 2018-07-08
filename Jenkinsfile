pipeline {
  agent any
  stages {
    stage('Move') {
      steps {
        sh '''rm -rf /var/jenkins_home/micro && mkdir /var/jenkins_home/micro

cp -rf * /var/jenkins_home/micro'''
      }
    }
  }
}