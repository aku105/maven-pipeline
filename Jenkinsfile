@Library('maven')_
pipeline {
    agent any
    stages{
        stage('Quality') {
             parallel{
                stage('Test'){
                    steps{
                        mavenTest 'M3'
                    }
                }
                stage('Sonar'){
                    steps{
                        try{
                            mavenSonar 'M3'
                        } catch(err) {
                            echo err
                        }
                    }
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
