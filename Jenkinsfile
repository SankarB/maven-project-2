pipeline {
    agent {label 'linux-slave-1' }
    stages {
        stage('Build') { 
            steps {
                echo 'build compilation'
                sh '/home/jenkins/maven-3.8/bin/mvn package'
            }
        }
        stage('Test') { 
            steps {
                echo 'TEst completed'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'binary deployed'
            }
        }
    }
}
