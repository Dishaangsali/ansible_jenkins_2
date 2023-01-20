pipeline {
    agent any
    stages {
        stage('Checkout from SCM') {
            steps {
                git credentialsId: '9ecc6334-6f72-4490-b946-fc6104e12966', url: 'https://github.com/Dishaangsali/ansible_jenkins_1.git'
            }
        }
        stage('Build') {
            steps {
                bat 'ansible-playbook playbook.yaml'
            }
        }
    }
}
