pipeline {
			agent none 
			stages {
				stage('BUILD') {
					agent { label 'master' }
					steps {
						sh '''
							pwd
							sleep 5
							echo This is the fist stage: BUILD
						'''
					}	
				}
				
				stage('TEST') {
					agent { label 'agent' }
					steps {
						sh '''
							pwd
							sleep 5
							echo This is the fist stage: TEST
						'''
					}	
				}
				
				stage('DEPLOY') {
					agent { label 'master' }
					steps {
						sh '''
							pwd
							sleep 5
							echo This is the fist stage: DEPLOY
						'''
					}	
				}
			}
		}
