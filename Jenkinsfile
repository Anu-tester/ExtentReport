pipeline {
    agent any
tools {maven 'Maven_3.5.2'} 
    stages {
        stage ('Compile Stage') {

            steps {
            
                    sh 'mvn clean'
                
            }
        }

        stage ('Testing Stage') {

            steps {
               
                    sh 'mvn clean install'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
                 
                    sh 'mvn deploy'
                
            }
        }
    }
}