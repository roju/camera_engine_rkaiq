# camera_engine_rkaiq

This code was shallow cloned from firefly sources with command:

```sh
git clone --depth 1 --branch rk356x/linux5.10_release_v1.2.1b https://gitlab.com/firefly-linux/external/camera_engine_rkaiq.git
```

Removed all "libgenMeshLib.a" files which are >100MB (github file size limit)

```sh
rm ./rkaiq/common/gen_mesh/android/genMesh_static_32bit/libgenMeshLib.a
rm ./rkaiq/common/gen_mesh/android/genMesh_static_64bit/libgenMeshLib.a
rm ./IspFec/src/gen_mesh/android/genMesh_static_32bit/libgenMeshLib.a
rm ./IspFec/src/gen_mesh/android/genMesh_static_64bit/libgenMeshLib.a
```

## Compiling

Native compile on RK3566:

```sh
./build.sh
```

### Tested platform

Hardware: Radxa Zero 3W (RK3566)\
System Image: Debian Bullseye (officially supported by Radxa)\
Camera: Radxa Camera 8M 219
