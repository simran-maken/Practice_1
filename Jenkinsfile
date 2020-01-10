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
		for ( int i = 0; i < 5; i++ )
		{
			stage("value: "+i){
				steps{
					if ( i%2 ==0 ){
						echo "even"
					}
					else{
						echo "odd"
					}
				}
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