# Atom editor for PHP in Docker container

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
