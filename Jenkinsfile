pipeline {
    agent any
    stage {
        steps{
     script {
        def mvnHome = tool 'maven-3'
    }
    }
    }
    
    stages {
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


        stage ('Deployment Stage') {
            steps {
                    sh 'mvn deploy'
                
            }
        }
    }
}
