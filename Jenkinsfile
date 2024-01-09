pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        echo 'commit the code'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploy the code'
      }
    }

    stage('config') {
      parallel {
        stage('config') {
          steps {
            echo 'config the code'
          }
        }

        stage('stage') {
          steps {
            echo 'stage the code'
          }
        }

      }
    }

  }
}