pipeline{
    agent: any
    environment {
        root = "go"
        branch = "main"
        scmUrl = "https://github.com/hariadiaf/sample-go-jenkins.git"
    }
    stages {
        stage("Go Version") {
            steps {
                sh "${root} version"
            }
        }
        stage("Git Clone") {
            steps {
                git branch: "${branch}", url: "${scmUrl}"
            }
        }
        stage("Go Test") {
            steps {
                sh "${root} test"
            }
        }
        stage("Go Build") {
            steps {
                sh "${root} build"
            }
        }
    }
}