pipeline{
    agent any
    stages{
        stage('Maven clean'){
            sh 'mvn clean'

        }
         stage('Maven install'){
            sh 'mvn install'
            
        }
         stage('Maven package'){
            sh 'mvn package'
            
        }
        
    }
}
    