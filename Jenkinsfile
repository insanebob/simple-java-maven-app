pipeline {
    agent {
       label 'container-slave'
    }
    stages {
        stage('Build') { 
            steps {   
                sh 'echo "Hello!!!"'
                sh 'mvn -B -DskipTests clean package'
                sh 'echo "Image Build finished!!"'
            }
        }
    }
}
