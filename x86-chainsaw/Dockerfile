FROM debian:jessie
#FROM debian:testing
MAINTAINER Necrose99 necrose99@protonmail.net
# ADD http://pc.cd/DzIrtalK /
# CMD ["/bin/bash"]
RUN echo "deb http://cdn.debian.net/debian/ testing main non-free contrib" >> /etc/apt/sources.list
RUN apt-get install --assume-yes locales
RUN locale-gen
RUN add-apt-repository  ppa:markhannon/ppa
RUN apt-get --assume-yes update
RUN apt-get --assume-yes upgrade
RUN apt-get --assume-yes install build-essential reprepro rsync wget zip git bzr mercurial install bash clonezilla docker.io drbl golang-go
RUN apt-get --assume-yes install csync pzip squashfs-tools zsync apt-utils bzip2 gcc apt-utils
ENV GOPATH /go
ENV PATH /usr/local/go/bin:$PATH:/go/bin
RUN apt-get clean
CMD ["/bin/bash"]

