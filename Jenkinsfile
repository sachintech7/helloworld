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
                bat 'java -jar target/*.jar'
            }
        }
    }
}

   
