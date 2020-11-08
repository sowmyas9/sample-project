pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compile stage...'
            }
        }
        stage('Package') {
            steps {
                echo 'Packaging stage...'
                echo 'Packaging stage...'
            }
        }
    
        stage('Testing') {
            steps {
                echo 'Testing stage...'
            }
        }
   
        stage('Deploy') {
            steps {
                echo 'Deploy stage...'
                echo 'Deploy stage...'
            }
        }
        stage('SonarQubeReport')
        {
            withSonarQubeEnv('MySonar') {
                sh "mvn sonar:sonar"
            }
        }
    }
}
