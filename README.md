# gitblit-docker
Simple dockerfile to host your own gitblit instance with Docker.

## Build the image

    docker build -t gitblit .

## Run the image

    docker run --rm -it --name gitblit -v /path/to/my/repos:/git -p 10080:8080 gitblit

Now you can open your gitblit instance at http://localhost:10080.

The gitblit instance is meant as a plain viewer for your repositories. It also *does not* update your repositories, so you have to keep an external script updating all repositories in the mounted directory.
