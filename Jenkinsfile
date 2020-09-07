pipeline {
  agent any
  stages {
    stage('Förbereda') {
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

    stage('Utföra') {
      steps {
        git(url: 'https://github.com/kemlo77/tabularasa', branch: 'master')
      }
    }

  }
}