# nss_with_nspr

*You must have gyp and ninja installed to build nss*

*https://gyp.gsrc.io/* 

steps to install GYP:
1) Install Chromium depot-tools
2) Add depot-tools to PATH
3) Use "fetch gyp" to instal gyp in current dir
4) Add gyp to PATH

-using GYP:

Example: **gyp_main.py <GypFileName.gyp> --depth .**
(This will build the passed gyp file that is located in the current dir)

*https://ninja-build.org/*

## build instructions:
1) enter nss subdir
2) use command: ./build.sh
3) build will be in dist dir
