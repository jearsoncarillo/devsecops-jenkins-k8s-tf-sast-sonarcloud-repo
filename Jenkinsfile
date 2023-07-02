pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=spsgbuggywebapp -Dsonar.organization=spsgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=30f5fb5c9836472fd355ce5a2e478cc9fe627296'
			}
        } 
  }
}
