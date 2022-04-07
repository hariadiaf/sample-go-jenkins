node {
    def root = "go"
    
        stage 'Checkout'
        git url: 'https://github.com/hariadiaf/sample-go-jenkins.git'
        
        stage 'preTest'
        sh "${root} version"
        
        stage 'Test'
        sh "${root} test ./... -cover"
        
        stage 'Build'
        sh "${root} build ./..."  
}