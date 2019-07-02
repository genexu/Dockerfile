# Watchman
![Docker Cloud Automated build](https://img.shields.io/docker/cloud/automated/genexu/watchman.svg)
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/genexu/watchman.svg)

Alpine base Facebook's Watchman container.

## Usage
```dockerfile
# Dockerfile
...
COPY --from=genexu/watchman /usr/local/bin/watchman* /usr/local/bin/
RUN watchman --trigger /path/to/dir 'trigger-name' -- trigger-command
...
```
