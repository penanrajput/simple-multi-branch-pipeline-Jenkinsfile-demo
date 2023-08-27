pipeline {
  agent any
  stages {
    stage('java stage') {
      steps {
			echo 'Hello, JDK'
			bat 'java -version'
      }
    }
    stage('maven stage') {
      steps {
			echo 'Hello, Maven'
			bat 'mvn -version'
      }
    }
  }
}