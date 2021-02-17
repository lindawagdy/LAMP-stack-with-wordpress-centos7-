pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      steps {
        sh 'echo Build'
      }
    }

    stage('Fluffy Test') {
      parallel {
        stage('Fluffy Test') {
          steps {
            sh 'echo Test'
          }
        }

        stage('frontend') {
          steps {
            echo 'stage1'
          }
        }

        stage('backend') {
          steps {
            echo 'stage2'
          }
        }

        stage('performance') {
          steps {
            echo 'stage3'
          }
        }

      }
    }

    stage('Fluffy Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}