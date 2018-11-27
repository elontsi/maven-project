pipeline {
	agent any
	
	stages{
		stage("Build"){
			steps{
				sh 'mvn clean package'
				sh "docker build /root/maven-project/webapp -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}

}

