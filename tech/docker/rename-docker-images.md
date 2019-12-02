# Rename Docker images

Docker images can easily be renamed (or their path or repository can be changed) by re-using the `docker tag` command:

```bash
$ docker tag [current image name or id] [new image name]
```

Example:

```bash
$ docker tag registry.example.com/group/project/website:latest registry.example.com/group/project/website:v1.0.0
```
