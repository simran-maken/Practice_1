pipeline{
	agent any
	stages{
		stage('stage 1'){
			echo "2222222222"
		}
		stage('stage 2'){
			build 'Java Project'
		}
		for ( int i = 0; i < 5; i++ )
		{
			stage("value: "+i){
				if ( i%2 ==0 ){
					echo "even"
				}
				else{
					echo "odd"
				}
			}
		}
		stage("stage parallel"){
			parallel{
				stage("aaaaaaaa"){
					echo "aaaaaa"
				}
				stage("bbbbb"){
					echo "sssss"
				}
			}
		}
	}
}