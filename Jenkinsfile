pipeline {
    docker { 
            image 'node:20.11.1-alpine3.19'
             // Run the container on the node specified at the
                    // top-level of the Pipeline, in the same workspace,
                    // rather than on a new node entirely:
            reuseNode true
                   
                   }
          }

    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
