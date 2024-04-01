pipeline {

    agent any

    stages {
         stage('build') {
          steps {
              bat 'npm install'
            }
          }

        stage('Docker Compose Up') {
            steps {

                    bat "docker compose up"

            }
        }
         stage('kill') {
            steps {

                    bat "docker compose down"

            }
        }
    }
}