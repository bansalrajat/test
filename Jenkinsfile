@Library('pipeline-library-demo')_

pipeline{
    agent { label 'master'}
        stages {
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
