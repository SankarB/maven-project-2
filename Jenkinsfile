pipeline {
    agent {label 'linux-slave-1' }
    stages {
        stage('Build') {
            sh "mvn package"
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
