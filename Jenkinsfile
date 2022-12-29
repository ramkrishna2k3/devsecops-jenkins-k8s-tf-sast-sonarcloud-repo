pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonarbuggywebapp -Dsonar.organization=sonarbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7d86f0d7e28087ede4a5cb8ceec7b382428c9ce7'
			}
        } 
  }
}
