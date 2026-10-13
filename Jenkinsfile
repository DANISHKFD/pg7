
pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                bat 'git -c safe.directory=D:/Projects/test/pg7/.git clone D:/Projects/test/pg7 repo'
            }
        }

        stage('Deploy') {
            steps {
                bat 'if not exist C:\\web mkdir C:\\web'
                bat 'copy repo\\index.html C:\\web\\index.html'
                echo 'Deployment successful!'
            }
        }
    }
}
