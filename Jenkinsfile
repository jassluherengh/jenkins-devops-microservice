pipeline{
	agent {
        docker { dir('C:\\Program Files (x86)\\Jenkins\\workspace\\jenkins-devops-microservice-pipeline') {
			image 'maven:3-alpine' }
    }
	stages{
		stage('Build'){
			steps{
				echo "Build"
			}			
		}
		stage('Test'){
			steps{
				echo "Test"
			}			
		}
		stage('Integeration Test'){
			steps{
				echo "Integeration Test"			
			}			
		}
	}
	post{
		always{
			echo "I am always called"
		}
		success{
			echo "build successful"
		}
		failure{
			echo "Build failed"
		}
	}

}