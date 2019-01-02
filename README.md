### About

The aim of this docker image is to set up an environment in which we can run
the Hyperion bit-level tests, to make sure that changes are not due to any
changes in environment but only changes in the code itself.

### Building

To build an image that will be uploaded to the Docker hub, use e.g.:

    docker build . -t astrofrog/hyperion-ci:<version>

where ``<version>`` is a version number that hasn't been used yet (e.g. ``1.6``)
used to identify the image. You can then push the image to the Docker Hub using:

    docker push astrofrog/hyperion-ci:<version>

