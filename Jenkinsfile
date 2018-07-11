// @Library('jenkins-dry-in-pipelines') _

pipeline {
    agent any
    stages{
        stage('eh'){
            steps{
                echo tool('jdk')
                echo tool('maven')
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
