pipeline{
    agent any {
        stages{
            stage("build"){
                steps{
                    echo("building the project")
                    sh "mvn clean package"
                }
            }
            stage(name: 'deploy')
            {
                echo("Deploying")
                echo("Deployed succesfully")
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
