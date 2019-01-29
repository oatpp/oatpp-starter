# oatpp-starter [![Build Status](https://dev.azure.com/lganzzzo/lganzzzo/_apis/build/status/oatpp.oatpp-starter?branchName=master)](https://dev.azure.com/lganzzzo/lganzzzo/_build/latest?definitionId=10?branchName=master)

oatpp simple-API starter project. 

More about oat++:
- Website: [https://oatpp.io](https://oatpp.io)
- Docs: [https://oatpp.io/docs/start](https://oatpp.io/docs/start)
- Oat++ Repo: [https://github.com/oatpp/oatpp](https://github.com/oatpp/oatpp)

## Overview

### Project layout

```

- CMakeLists.txt          // project loader script. load and build dependencies 
- main/                   // main project directory
    |
    |- CMakeLists.txt     // projects CMakeLists.txt
    |- src/               // source folder
    |- test/              // test folder

```
```
- src/
    |
    |- controller/              // Folder containing UserController where all endpoints are declared
    |- dto/                     // DTOs are declared here
    |- AppComponent.hpp         // Service config
    |- Logger.hpp               // Application Logger
    |- App.cpp                  // main() is here
    
```

---

### Build and Run

#### Using CMake

```
$ mkdir build && cd build
$ cmake ..
$ make run        ## Download, build, and install all dependencies. Run project

```

#### In Docker

```
$ docker build -t oatpp-starter .
$ docker run -p 8000:8000 -t oatpp-starter
```
