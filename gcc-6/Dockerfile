FROM Rikorose/gcc-cmake:gcc-6

RUN apt-get update && apt-get install -y --no-install-recommends \
    libgtest-dev \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

RUN wget https://github.com/nlohmann/json/releases/download/v2.0.8/json.hpp

RUN sudo mv -u json.hpp /usr/include/json.hpp