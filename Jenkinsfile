pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'Dev1'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test'
          }
        }

        stage('dep') {
          steps {
            echo 'Dep'
          }
        }

      }
    }

  }
}