pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                    
                    git branch: 'main', url: 'https://github.com/manojastro/demo-counter-app.git'
                }
            }
        stage('UNIt Testing'){
            
            steps{
                sh 'mvn test'
           }
      }
        stage('Intergration testing'){
            
            steps{
                sh 'mvn verify -DskipUnitTests'
    }
    
        
      }
        stage('Maven Build'){
            
            steps{
                sh'mvn clean install'
    } 
        }
}
}
