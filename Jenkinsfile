@Library('jenkins-dry-in-pipelines') _

pipeline {
    agent any
    stages{
        stage('Checkout') {
            steps{
                downloadSource()
            }
        }
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
