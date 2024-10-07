pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Makara1122/ansible_cdci.git'
            }
        }
        stage('Deploy') {
            steps {
                sh 'ansible-playbook -i inventory.yml playbook.yaml'
            }
        }
    }
}

