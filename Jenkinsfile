pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                    
                    git branch: 'main', url: 'https://github.com/manojastro/demo-counter-app.git'
                }
            }
        stage('UNIt Testing'){
            
            step{
                sh 'mvn test'
        }
        
    }
    }
}
