pipeline {
    agent any
    
    tools {
        maven 'maven_3.9'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package -DskipTests'
            }
        }
        
        stage('Run') {
            steps {
                bat 'java -jar target/helloworld-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}

   
