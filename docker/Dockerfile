FROM devwithlando/php:7.4-apache-2

ENV NODE_VERSION=12

# Install extra things for development purposes.
RUN wget -q https://www.browserstack.com/browserstack-local/BrowserStackLocal-linux-x64.zip && \
    unzip -d /usr/local/bin BrowserStackLocal-linux-x64.zip && \
    rm BrowserStackLocal-linux-x64.zip && \
    chmod +x /usr/local/bin/BrowserStackLocal && \
    curl -sL "https://deb.nodesource.com/setup_${NODE_VERSION}.x" | bash - && \
    apt-get install -y nano nodejs
