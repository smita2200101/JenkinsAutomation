pipeline {
    agent any

    stages {
        stage('First') {
            steps {
                echo "This is 1st stage"
            }
        }
        stage('Second') {
            when {
                expression {
                BRANCH_NAME=='Dev'
                }
            }
            
            steps {
                echo "This is 2nd stage"
            }
        }
        stage('Third') {
            steps {
                echo "This is 3rd stage"
            }
        }
        stage('Fourth') {
            steps {
                echo "This is 4th stage"
            }
        }
    }
    post {
        always {
        echo "This is always stage"
        }
        
    }
}
