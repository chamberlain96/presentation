pipeline {
    agent any  // Use any available agent (executor)
stages {
         stage('continuous download ') {
             steps  {
  git branch: 'main', credentialsId: 'qa', url: 'https://github.com/chamberlain96/presentation'
    // some block
    }
        }
        stage('Terraform Init and Apply') {
            steps {
                // Navigate to the Terraform code directory
                dir('Desktop/variable_tra/module/dev') {
                    // Run Terraform commands
                    sh 'terraform init'
                    sh 'terraform apply -auto-approve'
                }
            }
        }
    }
}
