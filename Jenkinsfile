pipeline {

    agent any
  tools {
        maven 'apache-maven-3_5_2' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }



          stage('deployment stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

}