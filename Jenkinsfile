pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Input'){
            steps{
                input 'Do you want to proceed?'
            }
        }
        stage('Output'){
            when{
                not{
                    branch 'master'
                }
            }
            steps{
                echo "Hello"
            }
        }
        
    }
}
