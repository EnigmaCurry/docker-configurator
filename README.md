# Docker Configurator

**DEPRECATED: I am now maintaining an updated version in [PlenusPyramis/dockerfiles/scripts/docker_configurator.py](https://github.com/PlenusPyramis/dockerfiles/blob/master/scripts/docker_configurator.py)**

This tool creates self-configuring docker containers given a single
YAML file.

Run this script before your main docker CMD. It will write fresh
config files on every startup of the container, based off of Mako
templates embedded in the docker image, as well as values specified in
a YAML file provided in a mounted volume.

The idea of this is that container configuration is kind of hard
because everyone does it differently. This creates a standard way of
doing it for containers that I write. A single file to configure
everything. 

You can see an example use of this in [lazy-distro-mirrors](https://github.com/EnigmaCurry/lazy-distro-mirrors)
