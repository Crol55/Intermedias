
pipeline{
    agent any 
    stages {

        stage ('Descargar dependencias'){
            steps{
                echo "dependencies" 
            }
        }
        stage ('Construir nuesta app'){
            steps {
                ansiblePlaybook credentialsId: 'private-key', disableHostKeyChecking: true, installation: 'Ansible2', inventory: 'dev.inv', playbook: 'ansible-playbook.yml'
            }
        }
    }

}