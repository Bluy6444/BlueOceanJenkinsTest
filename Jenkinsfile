pipeline {
  agent any
  stages {
    stage('Build Stage') {
      steps {
        echo 'Building the application'
      }
    }

    stage('Testing Stage') {
      parallel {
        stage('Testing Stage') {
          steps {
            echo 'Testing the application'
          }
        }

        stage('Test 1/2') {
          steps {
            echo 'Running first test'
          }
        }

        stage('Test 2/2') {
          steps {
            echo 'Running test 2'
          }
        }

      }
    }

    stage('Deploy Stage') {
      steps {
        echo 'Deploying the application'
      }
    }

  }
}