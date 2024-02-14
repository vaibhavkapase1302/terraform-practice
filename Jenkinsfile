pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', credentialsId: 'gitHub', url: 'https://github.com/vaibhavkapase1302/terraform-practice.git'
            }
        }
        stage('Terraform init') {
            steps {
                sh 'terraform init'
            }
        }
        stage('Terraform apply') {
            steps {
                sh 'terraform apply --auto-approve'
            }
        }
        
    }
}
