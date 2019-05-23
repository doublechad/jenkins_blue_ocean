pipeline {
  agent any
  stages {
    stage('version check') {
      steps {
        sh '''mvn --version
java -version'''
        tool(name: 'maven', type: 'maven')
      }
    }
    stage('git') {
      steps {
        git(url: 'https://github.com/doublechad/jenkins_blue_ocean.git', branch: 'master')
      }
    }
  }
}