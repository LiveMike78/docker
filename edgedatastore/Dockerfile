FROM ubuntu:18.04
WORKDIR /
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates libicu60 libssl1.0.0
ADD ./EdgeDataStore_linux-arm.tar.gz .
ENTRYPOINT ["./EdgeDataStore_linux-arm/OSIsoft.Data.System.Host"]
