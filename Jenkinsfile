pipeline {
    agent any
    environment {
        DIRECTORY_PATH = "https://github.com/mukulksingh98/SIT753-5.1P/new/main"
        TESTING_ENVIRONMENT = "Testing Environment"
        PRODUCTION_ENVIRONMENT = "mukulksingh"
    }
    stages {

        stage("Build") {
            steps {
                echo "fetch the source code from the directory path specified by the environment variable"
                echo "compile the code and generate any necessary artifacts"
            }
        }
        stage("Test") {
            steps {
                echo "Running unit tests for the application..."
                echo "Running integration tests for the application..."
            }
        }
        stage("Code Quality Check") {
            steps {
                echo "check the quality of the code for the application..."
            }
        }
        stage("Deploy") {
            steps {
                echo "deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage("Approval") {
            steps {
                echo "Approval stage..."
                sleep(time: 10, unit: 'SECONDS')
            }
        }
        stage("Deploy to Production") {
            steps {
                echo "Deploying to Production environment ${PRODUCTION_ENVIRONMENT}"
            }
        }
        

    }
}
