pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'mvn --version'
            sh 'ls'
          }
        }
        stage('') {
          steps {
            withMaven()
          }
        }
      }
    }
  }
}