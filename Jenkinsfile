pipeline {
  agent {label "linux"}

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh "mvn package"
                echo "Maven build completed Successfully"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
