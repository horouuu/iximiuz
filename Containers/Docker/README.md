# Docker
Container challenges related to Docker.
Thought I was familiar, but man did I have a lot to learn.

# [Easy] Build and Publish a Container Image With Docker (24/09/26)
<img src="./docker-registry-easy.png" width="400" alt="docker-registry-easy completion">

### Comments
This was a good starter. It was the first exercise I did, and I already felt \
like it was ironing out the wrinkles. I hadn't configured Docker registries all that often \
before this as I mostly worked on homelab configurations and I managed everything on one \
central device.
### Activities
- Authenticating to a toy Docker registry using `docker login`.
- Building a Docker image from a Dockerfile using `docker build`.
- Using the `-t` flag when building an image to tag the resultant image.
- Utilizing the naming convention of Docker images to push it to the toy registry with `docker push`.