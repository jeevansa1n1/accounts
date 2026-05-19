pipeline
{
	agent any
	
	stages{
		stage('Build app'){
			steps{
				sh 'mvn clean install'
			}
		}
		stage('Deploy app'){
			steps{
				sh 'mvn deploy -DmuleDeploclean install'
			}
		}
		stage('Testing app'){
			steps{
				sh 'newman run /Users/jeev/postman-collections/accounts-api-coll.postman_collection.json'
			}
		}
	}
}
		
		
		