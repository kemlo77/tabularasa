pipeline {
  agent any
  stages {
    stage('F�rbereda') {
      parallel {
        stage('Vakna') {
          steps {
            echo 'ring ring ring'
            timestamps() {
              sleep 10
            }

          }
        }

        stage('kliv upp') {
          steps {
            echo 'uppe'
          }
        }

      }
    }

    stage('Utf�ra') {
      steps {
        git(url: 'https://github.com/kemlo77/tabularasa', branch: 'master')
      }
    }

  }
}