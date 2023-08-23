pipeline{    
    agent any
    stages{
        stage('Git Checkout'){    
            steps{
                script {
                    
                    git 'https://github.com/meghaajoshi/webapp.git'
                }
            }
        }
        stage('UNIT Testing'){
            
            steps{
                
                script {
                    
                    sh 'mvn test'
                }
            }
        }
        stage('Integration Testing'){
            
            steps{
                
                script {
                    
                    sh 'mvn verify -DskipUnitTests'
                }
            }
        }
    }
)

