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
         stage ('send mail') {
           steps {    
               'mail bcc: '', body: 'The build is finished', cc: '', from: '', replyTo: '', subject: 'This is the build email', to: 'usntechnologies@gmail.com'
           }
       }
    }
}
