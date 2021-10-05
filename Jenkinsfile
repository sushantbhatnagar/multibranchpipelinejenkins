node {
  stage('Staging') {
    echo 'Test started'
  }

  stage('Test') {
    echo 'Test Completed'
  }

  stage('Deployment') {
    echo 'Test results deployed'
  }
  stage('cat README'){
    when {
      branch "fix-*"
    }
    steps {
      sh '''
        cat README.md
      '''
    }
  }
}
