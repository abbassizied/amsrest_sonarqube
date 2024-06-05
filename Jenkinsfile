pipeline {
    agent any 
    tools {
        maven 'maven383'
    }

    stages {
        stage('Build du Projet') {
            steps {
                sh 'mvn clean install -DskipTests'  
            }
        }
	    
        stage('Analyse Sonarqube') {
            steps {
	        withSonarQubeEnv(installationName: 'sq1') { 
		    sh 'mvn clean org.sonarsource.scanner.maven:sonar-maven-plugin:4.0.0.4121:sonar'
	        }
            }
        }
    }
}










