pipeline {
    agent {label 'linux-slave-1' }
    stages {
        stage('Build') {
        docker {
          /*
           * Reuse the workspace on the agent defined at top-level of Pipeline but run inside a container.
           * In this case we are running a container with maven so we don't have to install specific versions
           * of maven directly on the agent
           */
          reuseNode true
          image 'maven:3.5.0-jdk-8'
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
