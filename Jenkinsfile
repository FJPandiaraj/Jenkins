pipeline {
  agent none
  stages {
    stage('Example') {
      steps {
        echo 'Hello World'
        echo 'Message 2'
        node(label: 'master') {
          sh 'uname -a'
        }
        
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