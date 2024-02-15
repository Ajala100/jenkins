pipeline{
    agent any

    stages{
        stage('One'){
            steps {
                echo 'Step One is executing'
                }
           }
        stage('Two'){
             steps {
                echo 'Step Two is executing'
                }
          }

        stage('Three'){
               steps {
                  echo 'Step Two is executing'
                  }
               }
    }

     post {
            success {
                echo 'Pipeline succeeded! Triggering additional actions...'
                // Additional actions upon successful completion
            }
            failure {
                echo 'Pipeline failed. Notify the team...'
                // Notify the team or take corrective actions on failure
            }
        }

}