# Example-CRUD

A complete example of a "CRUD" service (UserService) built with Oat++. A modified version of [example-crud](https://github.com/oatpp/example-crud).

This example is tend to be built using vcpkg. Custom vcpkg ports were added to link with currently latest 1.3.0 oatpp libraries. Currently it's only tested on Windows with static linking and static crt (see vcpkg triplets).

### Build and Run

#### Pre Requirements

- Install vcpkg
- Add cmake.configureSettings to your IDE/editor with the following options:
  - CMAKE_TOOLCHAIN_FILE pointing to [vcpkg]/scripts/buildsystems/vcpkg.cmake
  - VCPKG_TARGET_TRIPLET - choose between x64-windows-custom and x86-windows-custom
  - VCPKG_OVERLAY_TRIPLETS pointing to triplets folder [root]/cmake/vcpkg/triplets
  - VCPKG_OVERLAY_PORTS pointing to ports folder [root]/cmake/vcpkg/ports

Run cmake and build
