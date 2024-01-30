pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asdbuggywebapp -Dsonar.organization=asdbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=52695e4d42eb966e05fb3b901406bc962a39678f'
			}
        } 
  }
}
