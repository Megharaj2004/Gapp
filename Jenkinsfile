pipeline{
	agent any
	tools{
		gradle 'gradle'
	}
	stages{
		stage('Checkout'){
			steps{
				git branch: 'master', url: 'https://github.com/Megharaj2004/Gapp'
			}
		}
		stage('Build'){
			steps{
				sh 'gradle build'
			}
		}
		stage('test'){
			steps{
				sh 'gradle test'
			}
		}
		stage('Run'){
			steps{
				sh 'gradle run'
			}
		}
	}
}
