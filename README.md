# dssat-docker
This is a docker image for the [DSSAT Cropping Systems Model](http://dssat.net/). It builds version 4.7.0.0 of the DSSAT CSM from bocinsky/bocin_base, an image including R and several command-line utilities.

### The Docker container

[Docker](https://www.docker.com/) is a virtual computing environment that facilitates reproducible research—it allows for research results to be produced independent of the machine on which they are computed. Docker users describe computing environments in a text format called a "Dockerfile", which when read by the Docker software builds a virtual machine, or "container". Other users can then load the container on their own computers. Users can upload container images to [Docker Hub](https://hub.docker.com/), and the image for this research is available at <https://hub.docker.com/r/bocinsky/dssat-docker/>.

#### Downloading and running the Docker container image

``` bash
docker run -it bocinsky/dssat-docker bash
```

#### Building the Docker container from scratch

If you wish to build the Docker container locally, clone this repository, `cd` into the `dssat-docker/` directory and run:

``` bash
docker build bocinsky/dssat-docker .
```

The `-t` argument gives the resulting container image a name. You can then run the container as described above.
