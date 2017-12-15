FROM centos/mysql-56-centos7
USER root
RUN yum -y update && yum -y install ansible
COPY assets/* /tmp/
RUN ansible-playbook /tmp/PacotesMysqlSei.yml
CMD ["/bin/sh"]
