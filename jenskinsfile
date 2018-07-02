pipline {
	agent any
	stages{
		stage('Compile Stage'){
			steps{
					withMaven(maven:'maven_3_5_4'){
					sh 'mvnw clean compile'
				}
			}

		}
		stage('Testing Stage'){
			steps{
				withMaven(maven:'maven_3_5_4'){
					sh 'mvnw test'
				}
			}
		}
		stage('Deployment Stage'){
			steps{
				withMaven(maven:'maven_3_5_4'){
					sh 'mvnw deploy'
				}
			}
		}
	}
}