node {
    stage('Clone repository') {
        /* Cloning the Repository to our Workspace */

        checkout scm
    }
    stage('build'){
        def customImage = docker.build("my-image")
    }
    stage('Test image') {
            app.inside {
                echo "Tests passed"
            }
}
}