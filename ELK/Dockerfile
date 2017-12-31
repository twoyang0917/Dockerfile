FROM twoyang0917/oracle-jdk-8:latest

RUN \
  wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | apt-key add - && \
  echo "deb https://artifacts.elastic.co/packages/6.x/apt stable main" > /etc/apt/sources.list.d/elastic-6.x.list && \
  apt-get update && \
  apt-get --no-install-recommends -y install logstash elasticsearch kibana && \
  rm -rf /var/lib/apt/lists/*

# Set environment variables.
ENV HOME /root

# Define working directory.
WORKDIR /root

# Define default command.
CMD ["tail", "-f", "/etc/hosts"]
