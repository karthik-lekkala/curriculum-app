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

        stage('front end unit') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}