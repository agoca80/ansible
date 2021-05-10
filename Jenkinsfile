pipeline {
    agent any 
    stages {
        stage('converge') { 
            steps {
                sh('
                    ansible-playbook -l lenovo   plays/lenovo.yml
                    ansible-playbook -l mountain plays/mountain.yml
                ')
            }
        }
    }
}
