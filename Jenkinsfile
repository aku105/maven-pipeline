@Library('maven')_
pipeline {
    agent any
    stages{
        stage('Pre-build') {
            parallel{
                steps{
                    mavenTest 'M3'
                    mavenSonar 'M3'
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
