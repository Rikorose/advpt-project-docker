FROM rikorose/gcc-cmake:gcc-4

RUN apt-get update && apt-get install -y --no-install-recommends \
    libgtest-dev \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

RUN wget https://github.com/nlohmann/json/releases/download/v2.0.8/json.hpp

RUN mv -u json.hpp /usr/include/json.hpp
