pipeline{
	agent any
	environment{
		Akey = "/var/lib/jenkins/ec2key.pem"
		ProdServer = "ec2-user@18.223.3.165"
		//user = 'ec2-user'
	}
	stages{
				
		stage('Create Docker Image'){
			steps{
				sh 'docker build -t tomsample .'
				//logcred = "${ProdServer}"
				//sh 'sudo su'
				//sh 'ssh ${ProdServer} -i ${Akey}'
				//sh 'sudo yum update'
				//sh 'whoami'}
			}
		}
		//stage('Testing'){
		//	steps{
		//	withMaven(maven: '3_1_2'){
		//	sh 'mvn test'}
		//	}
		//}
		//stage('Packaging'){
		//	steps{
		//	withMaven(maven: '3_1_2'){
		//	sh 'mvn install'}
		//	}
		//}
		//stage('PushToGit'){
		//	steps{
		//	def m = readMavenPom file: 'pom.xml'
		//	def groupId = m.groupId
		//	}
		//}
	
}
