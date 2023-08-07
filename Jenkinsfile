node {
    stage('Clone repository') {
        /* Cloning the Repository to our Workspace */

        checkout scm
    }
    node {
        checkout scm

        def customImage = docker.build("my-image")

        customImage.inside {
            sh 'make test'
        }
    }
}