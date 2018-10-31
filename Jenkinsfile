pipeline {
  agent any
  stages {
    stage('Test1') {
      steps {
        sh 'echo "HElloWorld"'
      }
    }
    stage('Test2') {
      steps {
        sh 'echo "Tutturu"'
      }
    }
    stage('ParallelCode') {
      steps {
        parallel(
        a: {
          echo "This is branch a"
        },
        b: {
          echo "This is branch b"
        }
      }
    }
  }
}
