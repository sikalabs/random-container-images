IMAGE=ttl.sh/image-updater-example

build-and-push:
	docker build -t $(IMAGE) --build-arg BUILD_IN_SUFFIX=`slr next-dev-docker-tag` .
	docker push $(IMAGE)
