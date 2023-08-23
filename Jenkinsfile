pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecgurubuggyapp -Dsonar.organization=asecgurubuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3dc3295706d2ba9898524fb3b8afdb9e374527d4'
			}
        } 
  }
}
