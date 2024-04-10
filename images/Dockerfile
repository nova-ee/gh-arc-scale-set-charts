FROM ghcr.io/actions/actions-runner:latest

RUN sudo apt-get update -y \
    && sudo apt-get install -y wget apt-transport-https software-properties-common \
    && sudo apt-get install -y --no-install-recommends \
    curl \
    ca-certificates \
    git \
    jq \
    sudo \
    unzip \
    zip \
    libfreetype6-dev \
    python3 

RUN wget -q https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb \
	&& sudo dpkg -i packages-microsoft-prod.deb \ 
	&& rm packages-microsoft-prod.deb \
	&& sudo apt-get update \ 
	&& sudo apt-get install -y powershell 
    
