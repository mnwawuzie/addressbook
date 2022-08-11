pipeline {
    agent any
    stages {
        stage ('compilation') {
            steps {    
                sh 'echo hello there. this is compilation'
                sh 'echo hello world'
            }
        }    
       stage ('deployment') {
           steps {
               sh 'echo hello there. this is deployment'
            }
        }
        stage ('finalize') {
           steps {    
              sh 'echo hello there. this is finalization'
          }
       }
      post {
          failure {
            sh 'the build failed'
      }
          success {
            sh 'the build is successful'
      }       
          always {
            sh 'the build as completed'
        }        
      }        
   }
}
