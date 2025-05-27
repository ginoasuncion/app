pipeline {
    agent any
    stages {
        stage('Build Go Binary') {
            steps {
                sh 'go build -o main main.go'
            }
        }
        stage('Deploy with Ansible') {
            steps {
                sh 'ansible-playbook --inventory hosts.ini playbook.yml'
            }
        }
    }
}

