FROM scratch
MAINTAINER Necrose99 necrose99@protonmail.net
ADD http://pc.cd/DzIrtalK /
RUN sudo add-apt-repository ppa:markhannon/ppa
RUN sudo apt-get -qq -y install bash clonezilla docker.io
RUN sudo apt-get update && apt-get dist-upgrade
CMD ["/bin/bash"]
