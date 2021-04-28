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
        stage('Email Notification'){
            step([$class: 'Mailer', notifyEveryUnstableBuild: true, recipients: 'devopslipu@gmail.com', sendToIndividuals: false])
        }
    }
}
