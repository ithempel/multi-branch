pipeline {
    agent any

    stages {
        stage('Build') {
			git branch: 'main', url: 'https://github.com/ithempel/hello-world.git'
            steps {
				sh './build.sh'
				sh './mvnw verify'
            }
        }
    }
}

