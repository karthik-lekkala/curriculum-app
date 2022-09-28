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
      parallel {
        stage('log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Irun 1') {
          steps {
            sh 'echo \'1\''
          }
        }

      }
    }

    stage('2') {
      steps {
        dir(path: '/home')
      }
    }

  }
}