pipeline {
    agent any
 
    tools {
        maven 'MAVE_HOME'
    }
 
stages{
        stage('Build'){
            steps {
                bat 'mvn clean package'
            }
            post {
                success {
                    echo 'Now Archiving test2...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }git 
        }
    }
}