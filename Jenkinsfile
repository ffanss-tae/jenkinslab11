pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/ffanss-tae/jenkinslab11.git', branch: 'master')
      }
    }

    stage('test') {
      steps {
        bat 'mvn clean test'
      }
    }

    stage('deliver') {
      steps {
        input 'deliver Done'
      }
    }

  }
}