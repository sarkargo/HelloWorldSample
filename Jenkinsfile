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
                echo" Building the application";
            }
        }
        stage('Unit-Test') { 
            steps {
                echo"Integration testing";
            }
        }
     }
}
