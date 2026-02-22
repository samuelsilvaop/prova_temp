FROM jenkins/inbound-agent:lts-jdk17
#a 21 possui vulnerabilidades críticas

USER root

RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    cmake \
    make \
    git \
    clang \
    clang-tidy \
    clang-format \
    lcov \
    pkg-config \
    libgtest-dev \
 && rm -rf /var/lib/apt/lists/*

RUN cd /usr/src/gtest && cmake . && make && cp lib/*.a /usr/lib || true

USER jenkins