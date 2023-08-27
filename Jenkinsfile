pipeline {
  agent any
  stages {
    stage('parallel stage') {
      parallel {
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
    stage('git stage') {
      steps {
        echo 'Hello, git'
        bat 'git --version'
      }
    }

    stage('javac stage') {
      steps {
        echo 'Hello, javac'
        bat 'javac -version'
      }
    }

  }
}