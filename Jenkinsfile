pipeline {
    agent any
    stages {
        stage('Deploy with Ansible') {
            steps {
                sh 'ansible-playbook --inventory hosts.ini playbook.yml'
            }
        }
    }
}

