FROM microsoft/vsts-agent:ubuntu-16.04-standard

RUN pip install --upgrade pip
RUN pip install setuptools
RUN pip install conan

RUN rm /usr/bin/gcc
RUN rm /usr/bin/g++
RUN add-apt-repository ppa:ubuntu-toolchain-r/test
RUN apt-get update && apt-get install -y gcc-7 g++-7
RUN ln -n /usr/bin/gcc-7 /usr/bin/gcc
RUN ln -n /usr/bin/g++-7 /usr/bin/g++

RUN apt-get update && apt-get install -y ninja-build
RUN conan config install https://github.com/bisect-pt/conan_config.git
