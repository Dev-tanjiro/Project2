node {

    checkout scm

    docker.withRegistry('dev113621','dev-docker') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
