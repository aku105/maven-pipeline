@Library('maven')_
pipeline {
    agent any
    stages{
        stage('Demo') {
            steps{
                mavenTest 'M3'
                mavenBuild 'M3'
                mavenSonar 'M3'
            }
        }
    }
}
