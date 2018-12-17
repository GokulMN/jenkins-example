pipeline {
    agent any
  
    stages {
         stage('build customer app code') { 
 steps {
  script {
        sh 'sudo apt install -y maven'
        sh 'mvn clean install'
    }
  }
 }
    
        
        stage ('Compile Stage') {

            steps {
                    sh 'mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {

                    sh 'mvn test'
                
            }
        }



    }
}
