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
                sh '''
					mvn sonar:sonar \
					-Dsonar.projectKey=ams_rest \
					-Dsonar.projectName="ams_rest" \
					-Dsonar.host.url=http://sonarqube-1:9000 
                '''
            }
        }

  
    }
}










