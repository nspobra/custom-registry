node {
    checkout scm
      
    docker.withRegistry('https://192.168.17.170:5001', 'gcr:[testuser]') {

        docker.image('hello-world-custom').inside {
            sh 'node --version'
        }
    }
}
