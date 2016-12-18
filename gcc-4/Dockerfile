FROM rikorose/gcc-cmake:gcc-4

#RUN apt-get update && apt-get install -y --no-install-recommends \
#    libgtest-dev \
#    libc6-dev \
#  && apt-get clean \
#  && rm -rf /var/lib/apt/lists/*

RUN wget https://github.com/google/googletest/archive/release-1.8.0.tar.gz
RUN tar xf release-1.8.0.tar.gz
RUN cd googletest-release-1.8.0
RUN cmake -DBUILD_SHARED_LIBS=ON .
RUN make
RUN cp -a googletest/include/gtest /usr/include 
RUN cp -a googlemock/gtest/lib* /usr/lib

RUN wget https://github.com/nlohmann/json/releases/download/v2.0.8/json.hpp

RUN mv -u json.hpp /usr/include/json.hpp
