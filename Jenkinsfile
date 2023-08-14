node {
    stage('Clone repository') {
        /* Cloning the Repository to our Workspace */

        checkout scm
    }
    stage('Test') {
            /* Running tests on your code */
            sh 'node test.js'
    }
    stage('build'){
        def customImage = docker.build("my-image")
    }
}