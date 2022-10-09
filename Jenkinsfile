pipeline {
    agent any
    environment {
            name = "test"
            url = "https://localhost:8080"
    }
    stages {
        stage('Example Build') {
            steps {
                echo 'Build Edildi'
            }
        }
        stage('Example Test') {
            steps {
                echo 'Test Edildi'
            }
        }
        stage('Example Deploy') {
            when {  
                    beforeAgent true
                    environment name: 'name', value: 'test'
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}
