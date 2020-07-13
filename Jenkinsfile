pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				echo "build"
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