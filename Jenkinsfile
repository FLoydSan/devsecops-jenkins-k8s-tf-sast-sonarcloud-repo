pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=floydsan_test-projct -Dsonar.organization=FloydSan -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=$SONAR_TOKEN'
			}
        } 
  }
}
