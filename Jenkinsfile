pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Compile stage...'
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
            steps {
                withSonarQubeEnv('MySonar') {
                    bat "mvn sonar:sonar"
                }
            }
        }
    }
}
