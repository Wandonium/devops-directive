build-dev:
	docker build -t react-app .

build-local:
	docker build \
	-t react-app-prod:local \
	--build-arg CADDYFILE=Caddyfile.local \
	--build-arg BASE_URL=http://localhost:5000/api \
	-f Dockerfile.production .

build-production:
	docker build \
	-t react-app-prod:prod \
	--build-arg CADDYFILE=Caddyfile.prod \
	--build-arg BASE_URL=https://mern.ngazi.media/api \
	-f Dockerfile.production .