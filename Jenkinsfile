pipeline{
    agent any
    stages{
        stage('Maven clean'){
            steps{

            sh 'mvn clean'
        }
         stage('Maven install'){
            steps{

            sh 'mvn install' 
             } 
        }
        
         stage('Maven package'){
            steps{
            sh 'mvn package'  
            } 
        }
      } 
  }  
}    
    