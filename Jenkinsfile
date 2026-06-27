pipeline {
    agent any
    tools {
        maven 'M3'  // tera Jenkins mein jo Maven tool configure kiya hai uska naam
    }
    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'M3') {
                    sh 'mvn clean install findbugs:findbugs'
                }
            }
        }
    }
}