node('built-in') {
    // some block
}
    stages {
        
 stage('continuous download ') {
   git 'https://github.com/chamberlain96/presentation'
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
