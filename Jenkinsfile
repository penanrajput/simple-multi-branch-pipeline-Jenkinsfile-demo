pipeline {
  agent any
  stages {
    stage('parallel stage'){
		parallel {
      
        steps {
          echo 'Hello, JDK'
          bat 'java -version'
        
      }
     
        steps {
          echo 'Hello, Maven'
          bat 'mvn -version'
        
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

    stage('vscode stage') {
      steps {
        echo 'Hello, vscode'
        bat 'code --version'
      }
    }

  }
}