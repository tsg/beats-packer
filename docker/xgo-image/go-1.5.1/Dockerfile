# Go cross compiler (xgo): Go 1.5.1 layer
# Copyright (c) 2014 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM tudorg/xgo-base

MAINTAINER Tudor Golubenco <tudor@elastic.co>

# Configure the Go packages and bootstrap them
RUN \
  export DIST_LINUX_64=https://storage.googleapis.com/golang/go1.5.1.linux-amd64.tar.gz && \
  export DIST_LINUX_64_SHA1=46eecd290d8803887dec718c691cc243f2175fe0 && \
  \
  export DIST_LINUX_32=https://storage.googleapis.com/golang/go1.5.1.linux-386.tar.gz && \
  export DIST_LINUX_32_SHA1=6ce7328f84a863f341876658538dfdf10aff86ee && \
  \
  export DIST_OSX_64=https://storage.googleapis.com/golang/go1.5.1.darwin-amd64-osx10.6.tar.gz && \
  export DIST_OSX_64_SHA1=02451b1f3b2c715edc5587174e35438982663672 && \
  \
  export DIST_WIN_64=https://storage.googleapis.com/golang/go1.5.1.windows-amd64.zip && \
  export DIST_WIN_64_SHA1=7815772347ad3e11a096d927c65bfb15d5b0f490 && \
  \
  export DIST_WIN_32=https://storage.googleapis.com/golang/go1.5.1.windows-386.zip && \
  export DIST_WIN_32_SHA1=bb071ec45ef39cd5ed9449b54c5dd083b8233bfa && \
  \
  $BOOTSTRAP
