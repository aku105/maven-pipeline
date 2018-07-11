@Library('jenkins-dry-in-pipelines') _

pipeline {
    agent any
    stages{
        stage('Test') {
            steps{
                mvnTest()
            }
        }
        stage('Package') {
            steps{
                mvnPackage()
            }
        }
    }
}
