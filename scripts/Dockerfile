FROM ghcr.io/tiacsys/bridle-dojo:default

USER root

RUN apt update && \
    DEBIAN_FRONTEND=noninteractive \
    apt install -y --no-install-recommends \
    curl


ARG USERNAME=ubuntu
ARG USER_UID=1000
ARG USER_GID=$USER_UID

# Create the user

# ********************************************************
# * Anything else you want to do like clean up goes here *
# ********************************************************

USER ubuntu

RUN mkdir -p /home/ubuntu/ws

# Launch bash shell by default
CMD ["/bin/bash"]
