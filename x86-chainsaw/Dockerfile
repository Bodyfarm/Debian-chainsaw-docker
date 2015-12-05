FROM debian:jessie
MAINTAINER Necrose99 necrose99@protonmail.net
# ADD http://pc.cd/DzIrtalK /
# CMD ["/bin/bash"]
RUN add-apt-repository  ppa:markhannon/ppa
RUN apt-get --assume-yes update
RUN apt-get --assume-yes upgrade
RUN apt-get --assume-yes install build-essential reprepro rsync wget zip git bzr mercurial install bash clonezilla docker.io drbl golang-go
RUN apt-get --assume-yes install csync pzip squashfs-tools zsync
ENV GOPATH /go
ENV PATH /usr/local/go/bin:$PATH:/go/bin
CMD ["/bin/bash"]
