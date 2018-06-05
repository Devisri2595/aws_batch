FROM amazonlinux:latest
RUN yum -y install which unzip aws-cli
ADD ./fetch_and_run/fetch_and_run.sh /usr/local/bin/fetch_and_run.sh
RUN chmod -R 777 /usr/local/bin/
WORKDIR /tmp
USER nobody
ENTRYPOINT ["/usr/local/bin/fetch_and_run.sh"]
