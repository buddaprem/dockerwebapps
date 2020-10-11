node {

    checkout scm

    docker.withRegistry('https://github.com/buddaprem/', 'docker') {

        def customImage = docker.build("prembudda/buildtest")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
