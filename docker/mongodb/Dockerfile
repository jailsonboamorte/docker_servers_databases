ARG MONGODB_VERSION

FROM mongo:${MONGODB_VERSION}

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install ntp nano