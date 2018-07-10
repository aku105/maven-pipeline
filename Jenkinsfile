@Library('shared-lib')_
pipeline {
    agent any
    stages{
        stage('Run Maven') {
            steps{
                maven(mavenName: 'm3')
            }
        }
    }
}
