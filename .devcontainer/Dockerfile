# Use the official Hugo image as a base
FROM klakegg/hugo:ext-alpine

# Install additional tools
RUN apk add --no-cache \
    git \
    bash

# Create a non-root user and set permissions
RUN adduser -D vscode
RUN chown -R vscode:vscode /src

# Switch to the non-root user
USER vscode

# Set the working directory
WORKDIR /src