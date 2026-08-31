pipeline{
    agent any
    environment{
        GIT_REPO = "https://github.com/orlandor99/Jenkins_day_6.git"
        BRANCH = "main"
    }
    stages{
        stage("Checkout & Inspect"){
            steps{
                git branch: "${BRANCH}", url: "${GIT_REPO}"
                sh '''
                    git branch
                    ls -l
                    cat README.md
                '''
            }
        }
    }
}