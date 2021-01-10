FROM ubuntu:20.04
LABEL maintainer="Mutsuhiro Iwamoto <mutsuhiro6@icloud.com>"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && \
		apt -y upgrade && \
		apt install -y apt-utils build-essential git tar curl zip unzip wget pkg-config intel-mkl && \
		export MKLROOT=/opt/intel/mkl && \
		cd /opt && \
		git clone https://github.com/microsoft/vcpkg.git && \
		cd vcpkg && \
		./bootstrap-vcpkg.sh && \
		./vcpkg install eigen3

