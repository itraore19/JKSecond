pipeline {
    
    agent any
    
    stages {
        
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }

         stage('Test') {
            steps {
                echo 'Testing stuff...'
            }
        }

        stage('Deploy') {
          steps {
               sh """
               echo "Deploying Code"
               """
           }
        }

    }
}
