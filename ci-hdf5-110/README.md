### Building

To build an image that will be uploaded to the Docker hub, use e.g.:

    docker build . -t astrofrog/hyperion-ci-hdf5-110:<version>

where ``<version>`` is a version number that hasn't been used yet (e.g. ``1.6``)
used to identify the image. You can then push the image to the Docker Hub using:

    docker push astrofrog/hyperion-ci-hdf5-110:<version>
