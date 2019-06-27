pipeline{
    agent {
        label 'windows'
    }
    triggers {
        cron '* * * * *'
    }
    stages{
        stage('Saludo'){
            steps{
                echo 'Hola'
            }
        }
        stage('Version'){
            steps{
                echo 'Version de maven'
            }
        }
        stage('Despedida'){
            steps{
                echo 'Adios'
            }
        }
    }
    post{
        always{
            echo 'PD: Salgo siempre'
        }
        success{
            echo 'Acabó sin problemas'
        }
        failure{
            echo 'Bufff.......'
        }
        changed{
            echo 'Esto ha cambiado !!!'
        }
        unstable{
            echo 'Estoy que no se si estoy'
        }
        regression{
            echo 'Antes iba y ahora no voy!'
        }
    }
}
