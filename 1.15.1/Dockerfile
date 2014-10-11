FROM scratch

MAINTAINER e2tox <e2tox@microbox.io>

ADD rootfs.tar /

WORKDIR /data

VOLUME /data

# Define default command.
EXPOSE 8080 28015 29015

ENTRYPOINT ["/usr/bin/rethinkdb"]
CMD ["--bind", "all", "-d", "/data"]