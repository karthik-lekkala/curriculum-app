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
        sh 'echo \'3\''
      }
    }

    stage('4') {
      steps {
        sh 'echo \'3\''
      }
    }

    stage('5') {
      steps {
        echo 'dswx'
      }
    }

    stage('6') {
      steps {
        sleep 10
      }
    }

    stage('9') {
      steps {
        echo 'done'
      }
    }

  }
}