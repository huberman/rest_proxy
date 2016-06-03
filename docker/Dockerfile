FROM java:8

MAINTAINER hubert.matthews@transformuk.com

ADD mule-standalone-3.7.0.tar.gz /opt

RUN ln -s /opt/mule-standalone-3.7.0 /opt/mule && mkdir -p /opt/mule/apps

COPY rest_proxy-1.0.0-SNAPSHOT.zip /opt/mule/apps/rest_proxy-1.0.0-SNAPSHOT.zip

# Define environment variables.
ENV MULE_HOME /opt/mule

# Define working directory.
WORKDIR /opt/mule

CMD [ "/opt/mule/bin/mule" ]

# Default http port
EXPOSE 8083
