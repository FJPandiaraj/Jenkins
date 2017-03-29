pipeline {
  agent none
  stages {
    stage('Example') {
      steps {
        echo 'Hello World'
        pwd(tmp: true)
        echo 'Message 2'
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