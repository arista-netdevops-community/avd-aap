VERSION = 5.2.2
MAJOR_VERSION = 5 # AVD follows semantic versioning
REPOSITORY = quay.io/mtache/avd-aap
# docker, podman
RUNTIME = docker

all: build push

build:
	ansible-builder build --container-runtime docker -v 3 --tag ${REPOSITORY}:${VERSION} ${REPOSITORY}:${MAJOR_VERSION}

push:
	${RUNTIME} push ${REPOSITORY}:${VERSION}
	${RUNTIME} push ${REPOSITORY}:${MAJOR_VERSION}
