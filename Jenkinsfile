pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build done '
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test is done '
          }
        }

        stage('test5') {
          steps {
            echo 'test5 is done'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'eploy is done '
      }
    }

    stage('check ') {
      steps {
        echo 'check is done '
        input(message: 'are u sure ?', ok: 'yes')
      }
    }

  }
}