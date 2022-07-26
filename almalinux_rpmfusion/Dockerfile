FROM almalinux:9
MAINTAINER nikruasutan
RUN dnf update -y
RUN dnf install dnf-plugins-core -y
RUN dnf config-manager --set-enabled crb
RUN dnf install https://dl.fedoraproject.org/pub/epel/epel-release-latest-$(rpm -E %rhel).noarch.rpm -y
RUN dnf install https://mirrors.rpmfusion.org/free/el/rpmfusion-free-release-$(rpm -E %rhel).noarch.rpm -y
