# Malscan CI Build Testing - GitLab CI Docker Image - CentOS 7 Variant
FROM centos:6
MAINTAINER Josh Grancell <jgrancell@malscan.org>
RUN yum install -y epel-release
RUN yum install -y file wget clamav clamav-update postfix which
RUN /bin/bash -l -c "mkdir -p /var/lib/malscan"
RUN /bin/bash -l -c "wget -P '/var/lib/malscan/' http://database.clamav.net/main.cvd"
RUN /bin/bash -l -c "wget -P '/var/lib/malscan/' http://database.clamav.net/daily.cvd"
RUN /bin/bash -l -c "wget -P '/var/lib/malscan/' http://database.clamav.net/bytecode.cvd"
