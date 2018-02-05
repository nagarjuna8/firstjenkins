pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build'
      }
    }
    stage('integrate') {
      steps {
        build(job: 'job', propagate: true)
      }
    }
  }
}