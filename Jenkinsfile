pipeline {
    
        
            agent { any { image 'maven:3.8.4-openjdk-11-slim' } }
           
     
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
