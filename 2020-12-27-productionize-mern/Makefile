build-dev:
	cd client && $(MAKE) build-dev
	cd server && $(MAKE) build

run-dev:
	docker-compose -f docker-compose-dev.yml up

build-local:
	cd client && $(MAKE) build-local
	cd server && $(MAKE) build

run-local:
	ENV=local docker-compose -f docker-compose-prod.yml up

build-production:
	cd client && $(MAKE) build-production
	cd server && $(MAKE) build

run-production:
	ENV=prod docker-compose -f docker-compose-prod.yml up

SSH_STRING:=wando@102.37.138.143

ssh:
	ssh ${SSH_STRING}

copy-files:
	scp -r ./* ${SSH_STRING}:/home/wando/docker-tut