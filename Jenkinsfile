pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Hussain7k/NodeJSRepo.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        bat 'npm install'
      }
    }
     
    
    stage('Deploying') {
      steps {
        bat 'node app.js'
      }
    }
  }
}
