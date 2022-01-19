pipeline {

    agent any
    options {
            timeout(time:1, unit:'HOURS')
        }
    parameters {
        string(name: 'aravind', defaultValue:'jenkins user',description: 'wellcome to jenkins')
        password(name:'PASSWORD',defaultValueAsSecret:'encrypted',description:'enter password')
    }
    stages {
        stage('parameters') {
            steps {
            echo "HI ${params.aravind}"
            echo "password ${params.PASSWORD}"
            } 
        }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
    post {
        always{
            echo 'build always'
        }
    }
}


