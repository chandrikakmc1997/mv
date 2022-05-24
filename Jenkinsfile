pipeline {
    agent any
    tools {
        maven 'maven'
      jdk 'java'
    }

    environment {
    PATH = "C://WINDOWS/SYSTEM32"
}
    stages {
        stage ('git') {
            steps {
            git 'https://github.com/chandrikakmc1997/mv.git'
        }
    }
        stage ('build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
