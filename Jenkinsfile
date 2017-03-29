pipeline {
  agent none
  stages {
    stage('Example') {
      steps {
        parallel(
          "Example": {
            echo 'Hello World'
            echo 'Message 2'
            node(label: 'master') {
              sh 'pwd && uname -a'
            }
            
            
          },
          "MyWork": {
            echo 'This is my Work'
            isUnix()
            sh 'pwd && uname -a'
            
          }
        )
      }
    }
  }
  post {
    always {
      echo 'I will always say Hello again!'
      
    }
    
  }
}