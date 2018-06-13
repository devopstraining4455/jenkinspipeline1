pipeline {

    agent any
    tools {
        mavenhome 'apache-maven-3.5.0'
        javahome 'jdk8'
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
