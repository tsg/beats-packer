# Go cross compiler (xgo): Go 1.5.1 layer
# Copyright (c) 2014 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM tudorg/xgo-deb6-base

MAINTAINER Tudor Golubenco <tudor@elastic.co>

# Configure the Go packages and bootstrap them
RUN \
  export DIST_LINUX_64=https://storage.googleapis.com/golang/go1.5.1.linux-amd64.tar.gz && \
  export DIST_LINUX_64_SHA1=46eecd290d8803887dec718c691cc243f2175fe0 && \
  \
  export DIST_LINUX_32=https://storage.googleapis.com/golang/go1.5.1.linux-386.tar.gz && \
  export DIST_LINUX_32_SHA1=6ce7328f84a863f341876658538dfdf10aff86ee && \
  \
  $BOOTSTRAP
