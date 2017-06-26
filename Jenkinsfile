pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'stage1'
      }
    }
    stage('stage2') {
      steps {
        parallel(
          "stage2": {
            echo 'stage2'
            
          },
          "stage2-1": {
            echo 'stage2-1'
            
          },
          "stage2-2": {
            echo 'stage2-2'
            
          }
        )
      }
    }
    stage('stage3') {
      steps {
        echo 'stage3'
      }
    }
  }
}