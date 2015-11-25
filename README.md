# gitblit-docker
Simple dockerfile to host your own gitblit instance with Docker

## Build the image

    docker build -t gitblit .

## Run the image
    docker run --rm -it --name gitblit -v /path/to/my/repos:/git -P gitblit
