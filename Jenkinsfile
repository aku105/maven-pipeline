@Library('maven')_
pipeline {
    agent any
    stages{
         stage('Test') {
                steps{
                    mavenTest 'M3'
                }
            }
            stage('Sonar') {
                steps{
                    mavenSonar 'M3'
                }
            }
        
        stage('Build'){
            steps{
                mavenBuild 'M3'
            }
        }
    }
}
