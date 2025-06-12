pipeline {
  agent any
  tools { 
        maven 'maven-3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-buggywebapp01 -Dsonar.organization=devsecops-buggywebapp01 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7f7fc23e3e13faa242f267a057252b4a280d920b'
			}
        } 
  }
}
