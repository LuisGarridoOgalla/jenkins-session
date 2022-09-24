pipeline{
    agent any

    enviornment{
        DEMO = '1.3'
    }

    stage{
        stage('stage-1'){
            steps{
                echo "this is the build number $BUILD_NUMBER of demo $DEMO"
                sh '''
                echo "Using a mult-line shell step"
                chmod +x test.sh
                ./test.sh
                '''
            }
        }
    }
}