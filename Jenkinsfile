pipeline {
    agent any

    stages {
        stage ('GIT checkout') {
            steps {
            git branch: 'main', url: 'https://github.com/NethajShanmugam/git-hook-springboot.git'
            }
        }

        stage ('Build') {
            steps {
                sh "mvn clean compile -f ./complete/pom.xml"
            }
        }
    } 
}
