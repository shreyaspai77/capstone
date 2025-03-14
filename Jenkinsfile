pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'building the project'
                sh 'mvn clean package'
            }
        }
        stage('deploy') {
            steps {
                echo 'Deploying'
                echo 'Deployed successfully'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
