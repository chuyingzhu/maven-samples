pipeline {
  agent any
  tools { 
      maven 'ALAN_MVN' 
      jdk 'ALAN_JAVA' 
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/chuyingzhu/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn clean'
        sh 'mvn test'
        sh 'mvn verify'
      }
    }

  }
}
