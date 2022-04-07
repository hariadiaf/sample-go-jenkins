node {
    def root = "go"
    
        stage 'Checkout'
        checkout git: 'https://github.com/hariadiaf/sample-go-jenkins.git'
        
        stage 'preTest'
        sh "${root} go version"
        
        stage 'Test'
        sh "${root} go test -cover"
        
        stage 'Build'
        sh "${root}go build ."
}