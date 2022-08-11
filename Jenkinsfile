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
      
        }        
      }        
   }
}
