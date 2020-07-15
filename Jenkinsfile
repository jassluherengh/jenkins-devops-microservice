pipeline{
	agent any
	enviroment{
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
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