# datascience-notebook

This is creating my own data-science notebook. Beyond the normal image it will also include tensorflow  and keras for use in all classes of Spring 2022.

[![Binder](https://mybinder.org/badge_logo.svg)](your-mybinder-link)

The built image is [hosted on Docker-Hub](link-to-your-dockerhub).

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
