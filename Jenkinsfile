pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        sh 'cd /opt'
      }
    }
    stage('QA') {
      steps {
        parallel(
          "QA": {
            echo 'This is QA Step'
            
          },
          "QA1": {
            echo 'QA1 step'
            
          }
        )
      }
    }
    stage('UAT') {
      steps {
        echo 'UAT Step'
      }
    }
    stage('Final') {
      steps {
        echo 'Complete'
      }
    }
  }
}