@Library('my_lib') _
pipeline{
    agent any
    stages{
        stage('git checkout'){
            steps{
                sh 'echo passed'
            }
        }
        stage('Unit test using maven'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Unit test using shared lib'){
            steps{
                mvnTest()
            }
        }
    }
}