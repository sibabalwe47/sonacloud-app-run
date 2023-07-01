pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sibabalwe47_rds-ec2-nodejs -Dsonar.organization=sibabalwe47 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e4dcdb1aec7e9356b86e95f46a029bdc94665385'
			}
        } 
  }
}
