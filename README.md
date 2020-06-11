
# Manifests for the Apalis TK1 Platform

## Download Sources

Create a working directory for the build and clone the source repositories.

```shell
$ mkdir apalis-tk1
$ cd apalis-tk1
$ repo init -u https://github.com/tszucs/apalis-tk1.git -m yocto-rocko
$ repo sync
```

## Initialize Build Environment

Source the shell script `ublox-init-build-env` in order to prepare the build environment as well as necessary configuration files under `build/`.

```shell
$ source ublox-init-build-env -b -m apalis-tk1
```

## Start Build Process

```shell
$ bitbake ublox-console-image
```

## References

* https://developer.toradex.com/products/apalis-tk1
