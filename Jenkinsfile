pipeline {
    agent {
       label 'container-slave'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'Hello'
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
