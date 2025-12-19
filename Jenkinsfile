@Library('Sharedlibrary') _

pipeline {
    agent any

    stages {
        stage('Say Hello') {
            steps {
                script {
                    hello('World')  // Calling the hello function from vars/hello.groovy
                }
            }
        }

        stage('Print Message') {
            steps {
                script {
                    // Calling the MyUtils class from src/com/example/MyUtils.groovy
                    com.example.MyUtils.printMessage('Shared library is awesome!')
                }
            }
        }
    }
}
