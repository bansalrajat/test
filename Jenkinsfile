pipeline {
    agent none
    stages {
        stage ('Back-end'){
            agent {docker {image 'maven:3-alpine'}}
            steps{
			sh 'echo "Host IP  is : `hostname -i`"'
            sh 'echo "$PWD"'
            sh 'mvn -v'
			}
			
			}
		stage ('Front-end'){
		agent {docker {image 'node:7-alpine'}}
		steps{
		sh 'echo "hostname -i is :  `hostname -i`"'
		sh 'echo $PWD'
		sh 'node -v'
		}
		}
		stage ('No-end'){
		agent {dockerfile true}
		steps{ sh 'echo dokcerdokce '}
		
		}
			
    }



}
