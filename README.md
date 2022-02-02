# datascience-notebook

This is creating my own data-science notebook. Beyond the normal image it will also include tensorflow tensorbaord and keras for use in all classes of Spring 2022.

[![Binder](https://mybinder.org/badge_logo.svg)](your-mybinder-link)

The built image is [hosted on Docker-Hub](link-to-your-dockerhub).

## Using this repo
### With `docker`
Build:

```bash
docker build fill-in-the-rest
# Should explain how to build the image, including tagging it
#this is the tag b020a0cf3b96 to be on an image we know should work
docker build --rm -t jupyter/my-datascience-notebook .
#this is renaming it for upload
docker tag jupyter/my-datascience-notebook kevinmunson/my-datascience-notebook

```

Run:

```bash

# - Should publish port 8888
# - Should mount the local directory as a volume in the
#   container's home directory
# - Should `--rm` container when done
# - Should use `-it` mode
docker run --rm -p 8888:8888 -it -v ${pwd}:/home/jovyan/work jupyter/my-datascience-notebook
```

### With `docker-compose`
Build and run:

```bash
docker-compose up
# - It should publish port 8888
# - It should mount the local directory as a volume in the container's
#   home directory
```
