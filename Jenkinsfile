node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com','tr_again') {

        def customImage = docker.build("devT/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
