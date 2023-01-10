pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nghoratkarsonar -Dsonar.organization=nghoratkarsonar -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=761c6aae7668bc7d1b22c5cf989dc90de08fa954'
			}
        } 
  }
}
