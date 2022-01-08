pipeline {
    
        agent { any }
            
           
     
    stages {
        stage('Build') {
            steps {
                echo 'Buildin stage'
                
            }
        }
        stage('Test') { 
            steps {
                echo 'Testing stage'
                
            }
            post {
                always {
                    echo 'post steps'
                }
            }
        }
    }
}
