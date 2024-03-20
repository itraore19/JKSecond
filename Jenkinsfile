pipeline {
    
    agent any
    
    stages {
        
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }

        stage('Deploy') {
          steps {
               sh """
               echo "Deploying Code"
               """
           }
        }
        
         stage('Test') {
            steps {
                echo 'Testing stuff...'
            }
        }

    }
}
