pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M398"
    }

    stages {
        stage('Echo Version') {
            steps {
                sh 'echo Print maven version'
                sh 'mvn -version'
            }
        }
      stage('Build') {
        step {
        sh 'mvn clean install'
        }
      }
    }
}
