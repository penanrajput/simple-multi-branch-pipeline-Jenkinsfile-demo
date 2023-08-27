pipeline {
  agent any
  stages {
    stage('java stage') {
      steps {
        sh 'java -version'
      }
    }
    stage('maven stage') {
      steps {
        sh 'mvn -version'
      }
    }
  }
}