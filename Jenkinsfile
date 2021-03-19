pipeline{
	//agent {
    //    docker {
    //        image 'maven:3-alpine'
    //    }
    //}
	agent any
	stages{
		stage('Build'){
			steps{
					sh 'mvn --version'
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