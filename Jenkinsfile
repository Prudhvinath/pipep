pipeline { 
    agent any  
    stages { 
        
          stage('One') { 
            steps { 
               echo 'This is a minimal pipeline.'
              
               echo 'Memories of Alhambara.'
            }
        }
         stage('Two') { 
            steps { 
               echo 'check.'
              
                input('Do you want to  proceed?')
                
               echo 'sucdess.'
            }
        }
         
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.'
              
               echo 'Memories of Alhambara.'
            }
        }
        
        stage('Three') { 
            steps { 
               echo 'check3.'
              
                when {
                    not {
                        echo 'when condition fails'   
                    }
                  
                }
                
               echo 'success3.'
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
