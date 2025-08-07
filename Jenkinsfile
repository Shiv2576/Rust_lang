pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Shiv2576/Rust_lang'
            }
        }

        stage('Build') {
            steps {
                sh 'cargo build --verbose'
            }
        }

        stage('Test') {
            steps {
                sh 'cargo test'
            }
        }

        stage('Run') {
            steps {
                sh './target/debug/my-rust-project'
            }
        }
    }
}
