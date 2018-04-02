pipeline {
    agent none
    stages {
        stage ('Back-end'){
            agent {docker {image 'maven:3-alpine'}}
            steps{
			echo "Host IP  is :" `hostname -i` 
            echo "$PWD"
            sh 'mvn -v'
			}
			
			}
		stage ('Front-end'){
		agent {docker {image 'node:7-alpine'}}
		steps{
		echo "hostname -i is :  `hostname -i`"
		echo $PWD
		sh 'node -v'
		}
		}
			
    }



}
