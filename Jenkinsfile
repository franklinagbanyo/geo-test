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
                nexusArtifactUploader artifacts: [[artifactId: 'bioMedical',
                 classifier: '', file: '/target/bioMedical-0.0.2-SNAPSHOT.jar',
                  type: 'jar']], credentialsId: 'nexus-ID',
                   groupId: 'qa', nexusUrl: '18-209-44-106:8081',
                    nexusVersion: 'nexus3', protocol: 'http',
                     repository: 'frank-repo', version: '0.0.2-SNAPSHOT'
            }
        }
    }
 }