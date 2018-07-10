@Library('maven')_
pipeline {
    agent any
    stages{
        stage('Demo') {
            steps{
                mavenTest 'M2'
                mavenBuild 'M2'
                mavenSonar 'M2'
            }
        }
    }
}
