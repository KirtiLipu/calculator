pipeline{
    agent any
    stages{
        stage('Build/Compile'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Unit Test'){
            steps{
                sh "mvn test"
            }
        }
    }
}
