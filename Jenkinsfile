pipeline {
     agent any
     stages {
        
         stage('Building - Staging') {
              when {
                     branch 'POD-3'
                }
             
             steps {
                 echo 'Building from jenkins...'
             }
             post {
                 always {
                     jiraSendBuildInfo site : 'pod-wipro.atlassian.net'
                 }
             }
         }
        
        
     }
 }

      


        
       
    }
}
