pipeline {
    agent any
tools {maven 'MAVEN_HOME'} 
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