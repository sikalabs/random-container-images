IMAGE=ttl.sh/kargo-example

build-and-push:
	slr next-dev-docker-tag
	docker build \
		--build-arg BUILD_IN_SUFFIX=`slr next-dev-docker-tag --read` \
		-t $(IMAGE):`slr next-dev-docker-tag --read` \
		-t $(IMAGE) \
		.
	docker push $(IMAGE):`slr next-dev-docker-tag --read`
	docker push $(IMAGE)
