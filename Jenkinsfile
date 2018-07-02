pipeline {
	agent any
	tools {
        maven 'maven_3_5_4' 
    }
	stages{
		stage('Compile Stage'){
			steps{					 
					bat 'mvnw clean compile'				 
			}

		}
		stage('Testing Stage'){
			steps{
					bat 'mvnw test'
			}
		}
		stage('Deployment Stage'){
			steps{
					bat 'mvnw deploy'
			}
		}
	}
}