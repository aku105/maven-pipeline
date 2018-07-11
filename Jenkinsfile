@Library('jenkins-dry') _

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
                mvn "clean test"
            }
        }
        stage('Package') {
            steps{
                mvn "clean package"
            }
        }
    }
}
