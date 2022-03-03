node {

    checkout scm

    docker.withRegistry('https://hub.docker.com','4ee6e493-83bf-48c5-ab8a-84f59e81f603') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
