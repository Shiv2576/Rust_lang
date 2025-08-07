pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Shiv2576/Rust_lang'
            }
        }
        stage('Build') {
            steps {
                sh 'cargo build'
            }
        }
    }
}
