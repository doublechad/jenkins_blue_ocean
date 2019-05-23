pipeline {
  agent any
  stages {
    stage('version check') {
      steps {
        tool(name: 'maven', type: 'maven')
        sh 'mvn --vesion'
      }
    }
    stage('git') {
      steps {
        git(url: 'https://github.com/doublechad/jenkins_blue_ocean.git', branch: 'master')
      }
    }
  }
}