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
		successful{
			echo "build successful"
		}
		failed{
			echo "Build failed"
		}
	}

}