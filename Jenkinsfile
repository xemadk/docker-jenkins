pipeline {
    agent any
    environment {
        RELEASE='0.0.1'
    }

    stages {
        stage('Build'){
            agent any
            environment {
                LOG_LEVEL='INFO'
            }
            steps{
                echo "Building release ${RELEASE} with log level ${LOG_LEVEL}"
            }
        }
        stage('Test'){
            steps {
                echo "Testing. I can see release ${RELEASE} with log level ${LOG_LEVEL}"
            }
        }
    }
}