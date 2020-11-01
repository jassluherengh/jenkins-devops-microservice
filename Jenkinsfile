gitpipeline{
	agent any
//	environment{
//		dockerHome = tool 'myDocker'
//		mavenHome = tool 'myMaven'
//		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
//	}
	stages{
		stage('Build'){
			steps{
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
				echo "Integeration Test Jissu"			
			}			
		}
	}
	post{
		always{
			echo "I am awsome, I am always called"
		}
		success{
			echo "build successful When you are success"
		}
		failure{
			echo "Build failed"
		}
	}
}