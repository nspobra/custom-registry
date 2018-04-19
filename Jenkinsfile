node {
    checkout scm
      
    docker.withRegistry('https://192.168.17.170:5001') {

        docker.image('hello-world-custom').inside {
           sh 'make test'
        }
    }
}
