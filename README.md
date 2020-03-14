fontcustom-docker
-----------------

Fontcustom docker, updated in 2020

There are many other existing ones, but the libraries and dependencies are a bit out of date.

The existing ones:

* https://hub.docker.com/r/drichner/fontcustom/
* https://hub.docker.com/r/loremipsum/fontcustom/
* https://hub.docker.com/r/thomaswelton/fontcustom/

I tried to make the docker as minimal as possible by removing all dev packages, but cannot get it under 150 MB because of fontforge.

Usage:

`docker run --user="$(id -u):$(id -g)" -v ${PWD}:/project karel3d/fontcustom compile -n fontdir -h ./vectors/ -c config.yml`

TIP: use together with https://github.com/karel-3d/center-svg-docker for centering SVGs
