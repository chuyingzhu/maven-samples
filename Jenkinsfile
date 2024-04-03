pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/chuyingzhu/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean'
      }
    }

  }
}