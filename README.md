# Atom.io editor [![Docker Stars](https://img.shields.io/docker/stars/rakshazi/atom-editor.svg?maxAge=2592000)](https://hub.docker.com/r/rakshazi/atom-editor/)[![Docker Pulls](https://img.shields.io/docker/pulls/rakshazi/atom-editor.svg?maxAge=2592000)](https://hub.docker.com/r/rakshazi/atom-editor/)

### Usage (manual)

```bash
xhost +
docker run -d -v /tmp/.X11-unix/:/tmp/.X11-unix/ \
              -v /dev/shm:/dev/shm \
              -v `pwd`:/workspace \
              -e DISPLAY=${DISPLAY} \
              rakshazi/atom-editor
```

### Usage (replace native atom editor)
```
# curl -L https://raw.githubusercontent.com/rakshazi/docker-atom/master/atom >> /usr/local/bin/atom
# chmod +x /usr/local/bin/atom
```
