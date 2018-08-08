pipeline {
  agent any
  stages {
    stage('JamBuild') {
      parallel {
        stage('JamBuild') {
          steps {
            echo 'Hello Jam'
          }
        }
        stage('JamBuild2') {
          steps {
            sh '''./jenkins/build.sh
'''
          }
        }
      }
    }
    stage('JamTest') {
      steps {
        echo 'Test Jam'
        sleep 5
      }
    }
  }
}