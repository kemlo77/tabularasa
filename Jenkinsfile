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
      parallel {
        stage('R�ra') {
          steps {
            git(url: 'https://github.com/kemlo77/tabularasa', branch: 'master')
          }
        }

        stage('Blanda') {
          steps {
            sleep 2
          }
        }

      }
    }

    stage('Njuta') {
      parallel {
        stage('�ta') {
          steps {
            node(label: 'kenny')
            echo 'oj oj vad gott'
          }
        }

        stage('Diska') {
          steps {
            sleep 2
          }
        }

      }
    }

  }
}