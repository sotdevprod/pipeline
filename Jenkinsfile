pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Building..."'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo "Testing..."'
          }
        }

        stage('Test 2') {
          steps {
            sh 'echo "Testing...2"|'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Deploying..."'
      }
    }

  }
}