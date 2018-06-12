# eeag.docker

1. Get the docker installation repository and the source code:

		git clone git@github.com:eftafmo/eeag.docker.git



1. Starting the stack (production):

		cd eeag
		cp docker-compose.override-prod.yml.example docker-compose.override.yml
		cp web/web.prod.env.example web/web.env
		docker-compose up

1. Starting the stack (test):

		cd eeag
		cp docker-compose.override-test.yml.example docker-compose.override.yml
		cp web/web.test.env.example web/web.env
		docker-compose -p eeag_test up
