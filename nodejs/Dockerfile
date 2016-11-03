# 
# Refrences
# https://github.com/creationix/nvm
# 
# docker build -t centos-nodejs:boron .
# 

FROM centos-base:latest

# Install nvm and load env
RUN wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash

# Install node with nvm
RUN source ~/.bashrc \
    && nvm install lts/boron \
    && npm install -g npm cnpm

CMD ["/bin/bash"]
