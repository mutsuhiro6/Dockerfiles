# C++ for Linear Algebra Docker Image

This docker environment is to build & run C/C++ codes.

## Build & Run 

```
$ docker build -t $IMAGE_NAME:$TAG .
$ docker run -v path/to/project:/home/root --rm -ti $IMAGE_NAME:$TAG
```

## Installed Libraries

- Intel MKL (as native library)
- vcpkg (package manager for C++)
- Eigen3 (via vcpkg)

## References

- [Installing Intel MKL ...](https://software.intel.com/content/www/us/en/develop/articles/installing-intel-free-libs-and-python-apt-repo.html)
- [vcpkg: a C++ package manager for ...](https://docs.microsoft.com/en-us/cpp/build/vcpkg)

