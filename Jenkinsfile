pipeline {
	agent any
	tools
	{
		maven 'Maven'
		jdk 'JDK'
	}
	stages
	{
		stage('checkout')
		{
			steps
			{
				git 'https://github.com/Akashmishra1421/p1.git'
			}
		}
		stage('build')
		{
			steps
			{
				sh 'mvn clean package'
			}
		}
		stage('test')
		{
			steps
			{
				sh 'mvn test'
			}
		}
		stage('run')
		{
			steps
			{
				sh 'java-jar target/p1-1.0-SNAPSHOT.jar'
			}
		}
	}
}
	
	
	
	
