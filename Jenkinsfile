node {
    	checkout scm

    	docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("reactfe")

        customImage.push()
    }
}
