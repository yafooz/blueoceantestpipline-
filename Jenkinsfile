pipeline {
  agent any
  stages {
    stage('build ') {
      steps {
        echo 'build done '
      }
    }

    stage('test1 stages ') {
      parallel {
        stage('test1 stages ') {
          steps {
            echo 'test 1 stage'
          }
        }

        stage('test1 check') {
          steps {
            echo 'test1 checking'
          }
        }

        stage('running test2 ') {
          steps {
            echo 'test2 running '
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment is don e'
        input(message: 'are you sure to deploy?', ok: 'yes. sure.')
      }
    }

  }
}