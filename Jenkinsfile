pipeline {
  agent any
  options{
    buildDiscarder(logRotator(numToKeepStr:'5'))
  }
  stages {
    stage('FÃ¶rbereda') {
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

    stage('UtfÃ¶ra') {
      parallel {
        stage('Röra') {
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
        stage('Äta') {
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
