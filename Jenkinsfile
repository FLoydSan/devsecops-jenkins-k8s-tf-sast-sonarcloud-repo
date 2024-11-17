pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=floydsan_test-projct -Dsonar.organization=FloydSan -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e1a6f14ad0865a71c1a5d9132420b6cfe81dd5db'
			}
        } 
  }
}
