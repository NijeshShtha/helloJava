pipeline {
    agent none

    stages {
        stage('Frontend') {
            agent{
                label 'java-agent'
            }
            steps {
                dir('js'){
                   sh 'node helloWorl.js'
                }
            }
        }
        stage('Backend'){
            agent{
                lable 'java-script-agent'
            }
            steps{
                dir('java'){
                    sh 'java Helloworld.java'
                }
            }
        }
    }
}