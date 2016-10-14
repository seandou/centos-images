# 
# https://github.com/CentOS/sig-cloud-instance-images
# https://github.com/CentOS/CentOS-Dockerfiles
# 
# docker build -t centos-base .

FROM centos:7.2.1511

# Use aliyun repo
ADD CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo
ADD epel.repo /etc/yum.repos.d/epel.repo

RUN yum makecache fast \
    && yum -y --setopt=tsflags=nodocs update \
    && yum clean all

# RUN yum -y --setopt=tsflags=nodocs install epel-release \
#     && yum makecache fast && \
#     && yum clean all

# 
RUN yum -y --setopt=tsflags=nodocs install \
    net-tools wget telnet tree bash-completion vim git \
    htop nmap lsof nc \
    && yum clean all

# Set timezone
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

CMD ["/bin/bash"]
