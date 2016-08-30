# docker-asciinema

Dockerfile for asciinema. An easy way to record screen-casts.

## Usage

You probably want some dependencies for your screencast. You can do
your own Dockerfile with:

```
FROM paulbellamy/asciinema

RUN apt-get install -y my-dependencies
ADD custom-files ...
```

First, build the image:

```
$ docker build -t my-screencast .
```

Then, start recording:

```
$ docker run -ti my-screencast
```
