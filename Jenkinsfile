pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '/home/damodar/Downloads/apache-maven-3.6.3/bin/mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }

    }
}
