FROM kalilinux/kali-linux-docker 

MAINTAINER Simon Giguere "gigsim@gmail.com"

RUN echo "deb http://http.kali.org/kali kali-rolling main contrib non-free" > /etc/apt/sources.list && \
echo "deb-src http://http.kali.org/kali kali-rolling main contrib non-free" >> /etc/apt/sources.list

ENV DEBIAN_FRONTEND noninteractive 

RUN apt-get -y update && apt-get -y dist-upgrade && apt-get clean

CMD ["/bin/bash"]

VOLUME ["/srv/docker/hack/kali/:/etc/"]
