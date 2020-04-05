pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    //image 'maven:3-alpine'
                    label 'container-slave'
                    args '-v /root/.m2:/root/.m2' 
                }
            }
            steps {
                sh 'Hello!!'
                sh 'echo Going to build the package now!!'
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
