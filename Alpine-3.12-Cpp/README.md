# C/C++ Docker Image with Alpine Linux v3.12

## Build & Run Image

```
$ docker build -t $IMAGE_NAME:$TAG .
$ docker run -v path/to/project:/home/root --rm -ti $IMAGE_NAME:$TAG
``` 

## Installed 

- [git](https://pkgs.alpinelinux.org/package/v3.12/main/x86/git)
- [make](https://pkgs.alpinelinux.org/package/v3.12/main/x86/make) 
- [g++](https://pkgs.alpinelinux.org/package/v3.12/main/x86/g++)

## References

- [alpine - Docker Hub](https://hub.docker.com/_/alpine)
- [Alpine Linux packages](https://pkgs.alpinelinux.org/packages)

