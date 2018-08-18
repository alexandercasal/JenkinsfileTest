pipeline {
    agent any
    
    stages {
        stage("Development") {
            when { 
                changeRequest target: 'master' 
            }
            steps {
                echo 'TODO: Run build for PR'
            }
        }
        stage("Alpha") {
            when {
                branch 'master'
            }
            steps {
                echo 'Run build for Alpha and upload to play store'
            }
        }
        stage("Beta") {
            when {
                branch 'beta'
            }
            steps {
                echo 'Run build for Beta and upload to play store'
            }
        }
    }
}
