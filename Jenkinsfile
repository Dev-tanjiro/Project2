node {

    checkout scm

    docker.withRegistry('https://login.docker.com/u/login','dev-docker') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
