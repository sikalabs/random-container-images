build-and-push:
	slr next-dev-docker-tag

	docker build --platform linux/amd64 \
		-t ghcr.io/sikalabsregistry/wip/ci \
		-t ghcr.io/sikalabsregistry/wip/ci:`slr next-dev-docker-tag --read` \
		.

	docker push ghcr.io/sikalabsregistry/wip/ci
	docker push ghcr.io/sikalabsregistry/wip/ci:`slr next-dev-docker-tag --read`

	@echo "Pushed ghcr.io/sikalabsregistry/wip/ci"
	@echo "Pushed ghcr.io/sikalabsregistry/wip/ci:`slr next-dev-docker-tag --read`"
