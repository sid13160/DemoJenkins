pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        bat 'cd'
      }
    }

    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            timestamps() {
              echo 'That\'s fine'
            }

          }
        }

        stage('parallel_test') {
          steps {
            echo 'Parallel Print'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed on Prod'
      }
    }

  }
}