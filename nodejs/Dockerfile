# 
# Refrences
# https://github.com/creationix/nvm
# 
# docker build -t centos-nodejs:v6.9.1 .
# 

FROM centos-base:latest

RUN wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash

RUN source ~/.bashrc

RUN nvm install v6.9.1

RUN npm install -g npm cnpm

CMD ["/bin/bash"]