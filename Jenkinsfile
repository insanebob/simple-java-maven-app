pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            label 'container-slave'
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo Going to build the package now!!'
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
