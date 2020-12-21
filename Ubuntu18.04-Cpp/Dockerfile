FROM ubuntu:18.04
RUN apt update && \
		apt -y upgrade && \
		apt install -y build-essential git tar curl zip unzip wget pkg-config && \
		wget https://apt.repos.intel.com/intel-gpg-keys/GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB && \
		apt-key add GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB && \
		rm GPG-PUB-KEY-INTEL-SW-PRODUCTS-2019.PUB && \
		wget https://apt.repos.intel.com/setup/intelproducts.list -O /etc/apt/sources.list.d/intelproducts.list && \
		sh -c 'echo deb https://apt.repos.intel.com/mkl all main > /etc/apt/sources.list.d/intel-mkl.list' && \
		apt update && \
		apt -y install intel-mkl-2020.0-088 && \
		export MKLROOT=/opt/intel/mkl && \
		cd /opt && \
		git clone https://github.com/microsoft/vcpkg.git && \
		cd vcpkg && \
		./bootstrap-vcpkg.sh && \
		./vcpkg install eigen3 && \
		cd 

