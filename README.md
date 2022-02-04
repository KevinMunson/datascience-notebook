# datascience-notebook

This is creating my own data-science notebook. Beyond the normal image it will also include tensorflow  and keras for use in all classes of Spring 2022.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KevinMunson/datascience-notebook/HEAD)

The built image is [hosted on Docker-Hub](https://hub.docker.com/layers/kevinmunson/my-datascience-notebook/latest/images/sha256:fcc8c98fe3672dfdbb84f8e5060a4d0177216ce28a094e53bc91188256954eb6).

## Using this repo
### With `docker`
Build:

```bash

# run this command to build the image

docker build --rm -t jupyter/my-datascience-notebook .
#this is renaming it for upload

#This is tagging the image
docker tag jupyter/my-datascience-notebook kevinmunson/my-datascience-notebook

```

Run:

```bash

# - This publishes on port 8888
# - It mount the local directory as a volume in the
#   container's home directory
# - It `--rm` container when done
# - It uses `-it` mode meaning you can cancel when you want
docker run --rm -p 8888:8888 -it -v ${pwd}:/home/jovyan/work jupyter/my-datascience-notebook
```

### With `docker-compose`
Build and run:

```bash
docker-compose up


```
