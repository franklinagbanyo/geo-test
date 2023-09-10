pipeline{
    agent any
    stages{
       tools{
        maven '/opt/maven'
        }
        stage('maven clean'){
            steps{
                sh 'mvn clean'
            }
        }
        stage('maven install'){
            steps{
                sh 'mvn install'
            }
        }
        stage('maven package'){
            steps{
                sh 'mvn package'
            }
        }
        
    }
}
    
    