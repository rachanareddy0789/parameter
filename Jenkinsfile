pipeline {
	agent any
	triggers {
		cron('H/15 * * * *')
	}	
	stages {
		stage('BUILD') {
			steps {
				sh 'echo this is my first stage in pipeline job'
				sh 'ls -lrt'
				sh 'sleep 5'
			}	
		}	
		stage('TEST') {
			agent any
			steps {
				sh ''' 
					sleep 5
					du -h 
				   '''
			}
		}
		
		stage('DEPLOY') {
			agent any
			steps {
				sh ''' 
					sleep 5
					du -h 
				   '''
			}
		}
}
}