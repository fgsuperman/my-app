pipeline {
    
        
            agent { docker { image 'maven:latest' } }
           
     
    stages {
        stage('Build') {
            steps {
                echo 'Buildin stage'
                sh 'mvn --version'
                
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
