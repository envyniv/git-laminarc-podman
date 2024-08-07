# Docker images for Laminar CI

Docker images with the latest version of [Laminar CI](https://github.com/ohwgiles/laminar).

Creates containers based on Debian, Alpine and a static Alpine build.
For each base, produces a laminard and laminarc, where laminard contains both the client and server, and laminarc is
client only.

The static build is really only useful for the client `laminarc`, as this can be easily copied into other images,
or used as a tool like:

    docker run --rm -e LAMINAR_HOST=host:port skyhisi/laminarc-static-latest show-jobs
