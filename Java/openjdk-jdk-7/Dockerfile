FROM twoyang0917/ubuntu:latest

RUN \
  apt-get update && \
  apt-get --no-install-recommends -y install openjdk-7-jdk && \
  rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

CMD ["tail", "-f", "/etc/hosts"]
