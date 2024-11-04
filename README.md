# camera_engine_rkaiq

shallow cloned from firefly sources with command:

```sh
git clone --depth 1 --branch rk356x/firefly-5.10 https://gitlab.com/firefly-linux/external/camera_engine_rkaiq.git
```

removed all files >100MB (github file size limit)

```sh
rm ./rkaiq/common/gen_mesh/android/genMesh_static_32bit/libgenMeshLib.a
rm ./rkaiq/common/gen_mesh/android/genMesh_static_64bit/libgenMeshLib.a
rm ./IspFec/src/gen_mesh/android/genMesh_static_32bit/libgenMeshLib.a
rm ./IspFec/src/gen_mesh/android/genMesh_static_64bit/libgenMeshLib.a
```

## Compiling

Native compile on RK3566:

```sh
mkdir build
cd build
cmake ..
sudo make
```

### Tested platform

Hardware: Radxa Zero 3W (RK3566)\
System Image: Debian Bullseye (officially supported by Radxa)\
Camera: Radxa Camera 8M 219
