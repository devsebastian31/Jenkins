pipeline {
    agent any  
    stages {
        stage('Clonar Repositorio') {
            steps {
                // Limpia el directorio de trabajo antes de clonar
                deleteDir()
                
                // Clona el repositorio desde GitHub
                checkout([$class: 'GitSCM', 
                          branches: [[name: 'master']], 
                          userRemoteConfigs: [[url: 'https://github.com/SebastianZhunaula/Jenkins']]])
            }
        }
        
        stage('Realizar otras acciones') {
            steps {
                // Aquí puedes agregar más pasos para construir, probar, etc.
                sh 'bash shell.sh'
            }
        }
    }
        
    post {
        always {
            // Puedes realizar acciones finales aquí, como limpiar o notificar.
            sh 'exit'
        }
    }
}
