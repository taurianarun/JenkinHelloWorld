pipeline {
    agent any 
    stages {
        stage('One') {
            steps {
                echo 'Step one executed'
            }
        }
        stage('Two') {
            steps {
                input('Do you want to proceed')
            }
        }
        stage('Three') {
            when {
                not {
                    branch "master"
                }
                
            }
            steps {
                echo "Hello IBM"
            }
        }
    }
}