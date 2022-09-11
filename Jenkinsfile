pipeline {
    agent {label 'linux-slave-1' }
    stages {
        stage('Build') {
            steps {
            sh "mvn package"
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
