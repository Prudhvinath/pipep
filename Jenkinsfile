pipeline { 
    agent any  
    stages { 
        
         
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.'
              
               echo 'Memories of Alhambara.'
            }
        }
        
        
        stage ('compile stage') {
            steps {
                sh 'mvn clean compile' 
            }
        }
        
        stage ('test') {
            steps {
                sh 'mvn test' 
            }
        }
        
        
        
    }
}
