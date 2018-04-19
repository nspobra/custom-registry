node {
    checkout scm
    environment {
        CRED1 = credentials("testuser")
    }      
    
    docker.withRegistry('https://192.168.17.170:5001', '$CRED1') {

        docker.image('hello-world-custom').inside {
           sh 'make test'
        }
    }
}
