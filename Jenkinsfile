pipeline
{
	agent any
	
	stages{
		stage('Build app'){
			steps{
				sh '/opt/homebrew/bin/mvn clean install'
			}
		}
		stage('Deploy app'){
			steps{
				sh '/opt/homebrew/bin/mvn deploy -DmuleDeploclean install'
			}
		}
		stage('Testing app'){
			steps{
				sh '/opt/homebrew/bin/newman run /Users/jeev/postman-collections/accounts-api-coll.postman_collection.json'
			}
		}
	}
}
		
		
		