pipeline{
	agent { docker { image 'maven:3.6.3'} }
	stages{
		stage('Build'){
			steps{
				sh 'mvn --version' 
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