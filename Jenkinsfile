pipeline{
    agent{label "EC2-AWS"}
    stages{
        stage('Parar Ejecución'){
            steps{
                sh '''
                sudo docker compose down
                '''
            }
        }

         stage('Subir Servicio Ejecución'){
            steps{
                sh '''
                sudo docker compose up -d 
                '''
            }
        }
    }
}