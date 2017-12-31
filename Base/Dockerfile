FROM ubuntu:14.04

RUN \
  apt-get update && apt-get -y upgrade && \
  apt-get install -y build-essential && \
  apt-get install -y software-properties-common && \
  apt-get install -y apt-transport-https && \
  apt-get install -y python-dev && \
  apt-get install -y tmux curl git htop man unzip vim wget && \
  rm -rf /var/lib/apt/lists/*

RUN \
  wget https://bootstrap.pypa.io/get-pip.py && \
  python get-pip.py && \
  rm -f get-pip.py

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["tail", "-f", "/etc/hosts"]
