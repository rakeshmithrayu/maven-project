pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                bat 'mvn clean package'
                bat "docker build -t tomcatwebapp:${env.build_id}"
            }
            
        }
    }
}
