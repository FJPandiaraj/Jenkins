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
            node(label: 'master') {
              sh 'pwd && uname -a'
              echo 'Hello'
              pwd(tmp: true)
            }
            
            
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