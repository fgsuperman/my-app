pipeline {
    
        
            agent { docker { image 'maven:3.8.4-jdk-11'  } }
           
     
    stages {
        stage('Build') {
            steps {
                echo 'Buildin stage'
                sh 'mvn --version'
                sh 'mvn clean compile'
                
            }
        }
        stage('Test') { 
            steps {
                echo 'Testing stage'
                sh 'mvn test'
                
            }
            post {
                always {
                    echo 'post steps'
                }
            }
        }
    }
}
