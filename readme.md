Conan Boost Example
===================

Example of Boost.Asio using Conan

Files needed (included in this repo)
------------------------------------

- Source code: *async_tcp_echo_server.cpp*
- Build file: *CMakeListst.txt*
- Dependency file: *conanfile.txt*

Binary remotes
--------------

This projects uses conan packages from Bincrafters repository.
To add this remote to you Conan client do this:

``$ conan remote add bincrafters https://api.bintray.com/conan/bincrafters/public-conan``


```shell
$ conan --version
Conan version 2.7.0

$ conan profile show
Host profile:
[settings]
arch=armv8
build_type=Release
compiler=apple-clang
compiler.cppstd=20
compiler.libcxx=libc++
compiler.version=15
os=Macos

Build profile:
[settings]
arch=armv8
build_type=Release
compiler=apple-clang
compiler.cppstd=20
compiler.libcxx=libc++
compiler.version=15
os=Macos
```


```shell
$ cmake --version
cmake version 3.30.0

CMake suite maintained and supported by Kitware (kitware.com/cmake).
```

```shell
$ gcc --version
Apple clang version 15.0.0 (clang-1500.3.9.4)
Target: arm64-apple-darwin23.5.0
Thread model: posix
InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
```

```shell
$ g++ --version
Apple clang version 15.0.0 (clang-1500.3.9.4)
Target: arm64-apple-darwin23.5.0
Thread model: posix
InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
```

编译

```shell
$ ./build.sh
```

运行

```shell
$ ./run.sh
```
