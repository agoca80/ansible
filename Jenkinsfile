pipeline {
    agent any 
    stages {
        stage('converge') { 
            steps {
                sh('
                    ls
                    ansible-playbook plays/mountain.yml
                ')
            }
        }
    }
}