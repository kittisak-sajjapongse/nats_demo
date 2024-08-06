FROM ubuntu
RUN mkdir -p /data/nats.c; \
    apt-get update;\
    apt-get -y install git vim wget cmake build-essential libssl-dev libprotobuf-c-dev;\
    cd /data;\
    git clone https://github.com/nats-io/nats.c.git nats.c;\
    mkdir -p /data/nats.c/build; \
    cd /data/nats.c/build; \
    cmake ..;\
    make