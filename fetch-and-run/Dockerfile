FROM amazonlinux:latest
RUN yum -y install which unzip aws-cli
RUN chmod -R 777 /usr/local/bin/
COPY /var/lib/jenkins/workspace/aws_batch/fetch-and-run/fetch_and_run.sh /usr/local/bin/fetch_and_run.sh
WORKDIR /tmp
USER nobody
ENTRYPOINT ["/usr/local/bin/fetch_and_run.sh"]
