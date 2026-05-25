pipeline {
    agent none

    stages {
        stage('Frontend') {
            agent{
                docker{
                    image 'node:18'
                }
            }
            steps {
                dir('js'){
                   sh 'node helloWorl.js'
                }
            }
        }
        stage('Backend'){
            agent{
                docker {
                    image 'eclipse-temurin:17'
                }
            }
            steps{
                dir('java'){
                    sh 'java Helloworld.java'
                }
            }
        }
    }
}