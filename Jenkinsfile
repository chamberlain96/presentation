pipeline {
    agent any  // Use any available agent (executor)

    stages {
        stage('Continuous Download') {
            steps {
                // Checkout the code from GitHub
                git branch: 'main', credentialsId: 'qa', url: 'https://github.com/chamberlain96/presentation'
            }
        }

     stage('Checkout Code into Directory') {
            steps {
                // Use the 'dir' step to change the working directory
                dir('Desktop/variable_tra/module/dev') {
                    
      stage('Terraform Init and Apply') {
                        steps {
                            // Run Terraform commands
                            sh 'terraform init'
                            sh 'terraform apply -auto-approve'
                        }
                    }
                }
            }
    


 
