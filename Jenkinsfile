pipeline {
        agent any
        options {
            timeout(time:1, unit:'HOURS')
        }
        tools {
            maven 'apache-maven-3.8.4-bin.tar.gz'
        }
        stages {
            stage('version') {
                steps {
                    sh 'mvn --version'
                }
            }
        } 
}
