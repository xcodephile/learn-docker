FROM jenkins/jenkins:lts

USER root

# install npm and Smee (webhook payload delivery service)
RUN curl -fsSL https://deb.nodesource.com/setup_17.x | bash -
RUN apt update
RUN apt install -y nodejs
RUN npm install --global smee-client

# install screen to enable Smee run in background
RUN apt install -y screen

# install redis-cli command
RUN apt install -y redis-tools