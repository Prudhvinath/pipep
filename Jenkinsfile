pipeline { 
    agent any  
    stages { 
        
         stage ('Build') {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
        //stage('Build') { 
          //  steps { 
            //   echo 'This is a minimal pipeline.'
              
              // echo 'Memories of Alhambara.'
            //}
        //}
    }
}
