pipeline {
    agent any
    environment {
        DEMO = '1.3'
    }

    stages {
        stage('stage-1'){
            steps{
                echo "This is the build number $BUILD_NUMBER of $DEMO"
                sh '''
                    echo "Using multi line shell step"
                    chmod +x test.sh
                    ./test.sh
                '''
            }
        }
    }
}