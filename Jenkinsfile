pipeline {
agent any
stages{
	stage('build'){
		steps{
			sh 'echo "hello world"'
			sh '''
			echo "multiple shell steps works too"
			ls -lahss---
			'''
		}
	}
} 
post {
	always {
		echo "this will run always"
	}
	success {
		echo 'this will run only if successfull'
	}
	failure {
		echo 'this will run only if failure'
	}
	unstable {
		echo 'this will run only if build marks as a unstable'
	}
	changed {
		echo 'this will run only if pipeline state has changed'
	}
}	

}
