pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'Plan for Pipeline'
      }
    }

    stage('Code') {
      steps {
        echo 'Code for Pipeline'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build Pipeline'
          }
        }

        stage('Test') {
          steps {
            echo 'Test the Pipeline'
          }
        }

        stage('Release') {
          steps {
            echo 'Relaease'
          }
        }

        stage('Deploy') {
          steps {
            echo 'to deploy application'
          }
        }

        stage('Operate') {
          steps {
            echo 'to operate the app'
          }
        }

      }
    }

  }
}