# DevOps-Lab-2

The two files setup local GitLab, the Docker, and CI.

### The network problem:
* Runner doesn't know about the web part.
* Registration is needed: docker run --rm -it -v {./gitlab-runner/config}:/etc/gitlab-runner gitlab/gitlab-runner register --docker-network-mode gitlab_network

### Important note:
The current project makes use of "latest" keyword for fetching the latest version of the image, however such behavior is only used for demonstration purposes and in real projects fixed versions should be preferred to avoid behavioral inconsistencies.
