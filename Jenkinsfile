pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
				sh './build.sh'
				git branch: 'main', url: 'https://github.com/ithempel/hello-world.git'
				sh './mvnw verify'
            }
        }
    }
}

