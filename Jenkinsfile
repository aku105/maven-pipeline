@Library('maven')_
pipeline {
    agent any
    stages{
         stage('Test') {
             parallel{
                steps{
                    mavenTest 'M3'
                }
                                 steps{
                    mavenSonar 'M3'
                }
            }
         }
        stage('Build'){
            steps{
                mavenBuild 'M3'
            }
        }
    }
}
