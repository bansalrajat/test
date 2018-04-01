@Library('pipeline-library-demo')_

pipeline{
    agent any{
        stage('Demo') {
            steps{
                echo 'Hello world'
                sayHello 'Dave'
                }
        }
        stage('helloagain'){
            sayHello 'stage2'
            }
    }
    }
