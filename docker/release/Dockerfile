FROM selais/todobackend-base:latest
MAINTAINER Salam Y ELIAS <salamlinux@free.fr>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse