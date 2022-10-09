pipeline {
    agent { label 'MVN3' }
    stages {
        stage('scm') {
            steps{
            mail subject: 'Build Started',
                body: 'Build Started',
                to: 'boggarapusaigowtham@gmail.com'
            git branch:'develop',url:'https://github.com/GOWTHI143/nopCommerce.git'
            }
        }
        stage('build') {
            steps {
            sh "dotnet build"}
        }
    }
}