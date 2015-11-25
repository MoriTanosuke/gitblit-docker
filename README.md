# gitblit-docker
Simple dockerfile to host your own gitblit instance with Docker

## Build the image

    docker build -t gitblit .

## Run the image
    docker run --rm -it --name gitblit -v /path/to/my/repos:/git -p 10080:8080 gitblit

Now you can open your gitblit instance at http://localhost:10080.
