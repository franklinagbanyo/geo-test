pipeline{
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages{
        
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
        stage('upload jar file'){
            steps{
                sh 'curl --upload-file /var/lib/jenkins/workspace/maven-pipeline@2/target/bioMedical-0.0.2-SNAPSHOT.jar -u admin:devops -v http://ec2-18-209-44-106.compute-1.amazonaws.com:8081/repository/frank-repo/'
            }
        }
        
    }
}
    
    