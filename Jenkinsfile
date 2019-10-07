pipeline {
    agent any 
    stages {
        stage('Git-Checkout') { 
            steps {
                echo"Checking out code from Git";
                git credentialsId: 'admin', url: 'https://github.com/sarkargo/HelloWorldSample.git'
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package'
                echo "Build is Sucessfull";
            }
        }
        stage('Unit-Test') { 
            steps {
                echo"Integration testing";
            }
        }
     }
}
