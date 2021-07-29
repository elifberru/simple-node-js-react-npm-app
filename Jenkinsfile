node { 
  environment {
        CI = 'true' 
    }
	stage("Build") {
		sh 'docker pull 10.150.0.131/bitdevops/node:lts-buster-slim'
                sh 'npm install' 
	
	}
	stage('Test') { 
            steps {
                sh './jenkins/scripts/test.sh' 
            }
        }
	
	
}