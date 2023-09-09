pipeline{
    agent any
    stages { 
        stage ('maven clean') {
        steps{
            maven clean
        }
    }
        stage ( 'maven install'){
        steps{ 
            maven install   
        }
    }
        stage ( 'maven package'){
        steps{ 
            maven package   
        }
    }
    }
}
   