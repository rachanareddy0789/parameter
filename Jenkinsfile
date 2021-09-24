pipeline {
	agent { label 'master' }
	parameters {
		string(name: 'NAME', description: 'Enter your name here')
	}
	stages {
		stage('BUILD') {
			steps {
				echo "NAME ${params.NAME}"
				sh "echo ${params.NAME}"
				sh 'sleep 5'
			}	
		}	
		stage('TEST') {
			steps {
				sh ''' 
					sleep 5
					du -h 
				   '''
			}
		}
		
		stage('DEPLOY') {
			steps {
				sh ''' 
					sleep 5
					du -h 
				   '''
			}
		}
	}
}