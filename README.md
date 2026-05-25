## Docker image with ГОСТ git based on Slackware

ГОСТ git = GOST git. GOST ciphering = russian national cryptography standard.

Ready for CI/CD and fully compatible with ГОСТ ciphering.

__Components installed:__

- gcc
- __git with ГОСТ ciphering__
- cmake
- curl with ГОСТ ciphering
- OPENSSL with ГОСТ ciphering
- cppcheck
- gcovr
- gzip

### Usage

`git clone https://github.com/ujooju/slackware_cmake_image`

go to the slackware_cmake_image directory.

`docker build -t <any_name> .`

`docker run -it <any_name>`

### If you want to work wtih git server running with TLS1.2, execute the next command: 

_may be needed to work with ГОСТ ciphering_

`git config --global http.sslversion tlsv1.2`

### If there are some troubles with certificate verification, try this: 

__highly not recommended__

`git config --global http.sslverify false`



GOST git docker image.
