
pipeline{
    agent any 
    stages {

        stage ('Descargar dependencias'){
            steps{
                echo "dependencies" 
            }
        }
        stage ('Produccion-Ansible'){
            agent{
                label 'Ansible-aws-produccion'
            }
            steps {
                echo "hola mundo desde ansible"
                sh "whoami"
            }
        }
    }

}