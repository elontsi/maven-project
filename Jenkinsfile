pipeline {
	agent any
	
	stages{
		stage("Build"){
			steps{
				sh 'mvn clean package'
				sh "docker build /var/lib/jenkins/workspace/Tomcat -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}

}

