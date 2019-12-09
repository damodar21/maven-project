pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean pacakge'
            }

        post {
            success {
                echo "Now archiving"
                archiving artifacts: '**/target/*.war'
            }
        }
      }
    }
}
