node {
    checkout scm
      
    docker.withRegistry('https://192.168.17.170:5001', '${dockeruser}') {

        docker.image('hello-world-custom').inside {
            sh 'node --version'
        }
    }
}
