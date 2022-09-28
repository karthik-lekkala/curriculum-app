pipeline {
  agent any
  stages {
    stage('checkout Code') {
      steps {
        echo 'hello'
        git(url: 'https://github.com/karthik-lekkala/curriculum-app.git', branch: 'dev')
      }
    }

    stage('log') {
      steps {
        sh 'ls -la'
      }
    }

  }
}