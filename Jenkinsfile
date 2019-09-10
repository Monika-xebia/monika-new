pipeline {
agent any
stages{
	stage('build'){
		steps{
			sh echo "hello world"
			sh '''
			echo "multiple shell steps works too"
			ls -lah
			'''
		}
	}
} 
	

}
