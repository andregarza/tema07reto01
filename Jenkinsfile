pipeline {
    agent any
    stages{

        stage('Docker'){
            steps{
                echo 'Connecting with dockerserver-01'

            }

        }

        stage('build'){
            steps{
                echo 'Este stage sirve para compilar el código que fue obtenido del repositorio de Git'
                echo 'Su ejecución se dio gracias a que pasó correctamente el stage de Análisis'
            }

        }

        stage('DevOps config'){
            steps{
                echo 'Este stage sirve para conectar mediante variables de entorno, a otras herramientas de apoyo para asegurar la calidad del código'
                script{
                    env.USER_NAME = "Usuario"
                    env.USER_ID = "devops"
                }
                echo "Querido ${env.USER_NAME}"
                echo "Tu contraseña es: ${env.USER_ID}"
            }
        }


    }

}