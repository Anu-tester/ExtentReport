pipeline {
    agent any
tools {maven 'MAVEN_HOME'} 
    stages {
        stage ('Compile Stage') {

            steps {
            
                    sh 'mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {
               
                    sh 'mvn test'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
                 
                    sh 'mvn deploy'
                
            }
        }
    }
}