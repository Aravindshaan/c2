pipeline {
        agent any
        options {
            timeout(time:1, unit:'HOURS')
        }
        tools {
            maven 'apache-maven-3.6.3'
        }
        stages {
            stage(''version') {
                steps {
                    sh 'mvn --version'
                }
            }
        } 
}
