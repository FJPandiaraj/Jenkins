pipeline {
  agent none
  stages {
    stage('Example') {
      steps {
        echo 'Hello World'
      }
    }
  }
  environment {
    Name = 'Pandiaraj'
  }
  post {
    always {
      echo 'I will always say Hello again!'
      
    }
    
  }
}