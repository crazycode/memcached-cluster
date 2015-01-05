FROM crazycode/buildpack-deps
ADD source /twemproxy
RUN cd /twemproxy && \
    autoreconf -fvi && \
    ./configure && \
    make

ADD nutcracker.yml /etc/nutcracker.yml
