node('built-in') {
    // some block
}
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git branch: 'main', credentialsId: 'qa credentials ', url: 'git@github.com:chamberlain96/presentation.git'
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
