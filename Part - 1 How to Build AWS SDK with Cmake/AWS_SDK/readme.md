## About Complied File.
1. Refer [https://youtu.be/pXihGp-6V6I]
2. Windows 64bit
3. MSVC2017 64bit

### CMake Build Command
```
cmake <src AWS SDK source path> -G "Visual Studio 15 2017 Win64" -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=<Path to Store the .lib and .dll> -DBUILD_ONLY="s3;cognito-identity;transfer;awstransfer" -DAUTORUN_UNIT_TESTS=OFF -DENABLE_TESTING=OFF
```

### CMake ALL_Build Command
```
msbuild ALL_BUILD.vcxproj /p:Configuration=Debug 
```

### CMake INSTALL Command
```
msbuild INSTALL.vcxproj /p:Configuration=Debug
```

## Other Info
1. Here there will be only compiled files for debug and release
2. If you need source files of AWS SDK CPP, Refer [1], [2]

## AWS Link
[1] https://aws.amazon.com/sdk-for-cpp/

## AWS SDK CPP github Link
[2] https://github.com/aws/aws-sdk-cpp