pipeline {
    agent any
    environment {
            name = "test"
            url = "https://localhost:8080"
    }
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {             
                    environment name: 'name', value: 'test'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}
