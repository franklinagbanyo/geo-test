pipeline{
    agent any
    stages { 
        stage ('maven clean') {
        steps{
            sh 'mvn clean'
        }
    }
        stage ( 'maven install'){
        steps{ 
            sh 'maven install'   
        }
    }
        stage ( 'maven package'){
        steps{ 
            sh 'maven package'   
        }
    }
    }
}
   