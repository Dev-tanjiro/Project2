node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com','tr_again') {

        def customImage = docker.build("dev/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
