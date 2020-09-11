FROM ubuntu:latest

LABEL maintainer="tzeweiwee@gmail.com"

RUN apt-get update && apt-get -y install curl && apt-get -y install sudo
RUN curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
RUN curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl"
RUN chmod +x ./kubectl
RUN sudo mv ./kubectl /usr/local/bin/kubectl

CMD /bin/bash