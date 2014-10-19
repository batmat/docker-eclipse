Running Eclipse Luna inside a Docker container
---------------------------------------------

## Preliminary note
This image is heavily based on http://fabiorehm.com/blog/2014/09/11/running-gui-apps-with-docker/. 
Kudos to @fgrehm.

## TL;DR: how to use it

### Build the image if you don't trust the pullable one

    $ sudo docker build -t batmat/eclipse

### Run it

    $ sudo docker run -it -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix batmat/eclipse
