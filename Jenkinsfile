pipeline{
	agent any
	stages{
		stage('stage 1'){
			steps{
				echo "2222222222"
			}
		}
		stage('stage 2'){
			steps{
				build 'Java Project'
			}
		}
		stage("stage parallel"){
			parallel{
				stage("aaaaaaaa"){
					steps{
						echo "aaaaaa"
					}
				}
				stage("bbbbb"){
					steps{
						echo "sssss"
					}
				}
			}
		}
	}
}