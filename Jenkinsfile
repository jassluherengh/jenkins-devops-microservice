pipeline{
	agent any
	#agent {
    #    docker { image 'maven:3-alpine' }
    #}
	stages{
		stage('Build'){
			steps{
				echo "Build"
				echo "Path -$PATH "
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