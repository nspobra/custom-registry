node {
    checkout scm

    docker.withRegistry('https://192.168.17.170:5001', 'testuser-registry') {

        docker.image('my-image').inside {
            sh 'node --version'
        }
    }
}
