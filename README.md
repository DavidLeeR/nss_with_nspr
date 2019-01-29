# nss_with_nspr

*******************************************************************************************************

## PREREQUISITES:

*You must have gyp and ninja installed to build nss*


### Install GYP:

*https://gyp.gsrc.io/* 

1) Install Chromium depot-tools
2) Add depot-tools to PATH
3) Use "fetch gyp" to instal gyp in current dir
4) Add gyp to PATH

### Install ninja:

*https://ninja-build.org/*

1) Follow instructions on ninja site above


********************************************************************************************************
## BUILD SIGNTOOL(and nss, zlib library, and jar library along the way):
*all build steps have already been completed in this repo

### 1. build nss instructions (already built (dist dir) in this repo):
1) navigate to nss subdir
2) use command: **./build.sh**
3) build will be in dist dir

### 2. build zlib instructions
1) navigate to nss/lib/zlib subdir
2) use command: **make**
3) .o and .a files found in current dir
4) drag libnss_zlib.a to dist/Debug/lib subdir

### 3. build jar library instructions
1) navigate to nss/lib/jar subdir
2) use command: **make**
3) .o and .a files found in current dir
4) drag libjar.z.a to dist/Debug/lib subdir

### 4. build Signtool instructions:
1) ensure nss has been built (step 1) (ie. ensure dist dir exists)
2) ensure zlib and jar libraries have been built and respective .a files placed in dist/Debug/lib subdir (steps 2 and 3) 
2) navigate to nss/cmd/signtool dir
3) use command: **make**

****************************************************************************************************************************
## CLEAN INSTRUCTIONS:

### clean nss instructions:
1) delete dist dir

### clean zlib library instructions
1) navigate to nss/lib/zlib subdir
2) use command **make clean**

### clean jar library instructions
1) navigate to nss/lib/zlib subdir
2) use command **make clean**

### clean Signtool instructions:
1) navigate to nss/cmd/signtool subdir
2) use command **make clean**
