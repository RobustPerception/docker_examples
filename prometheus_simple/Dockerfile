# Simple example of how to specify configuration files.

# Use the main Prometheus image.
FROM prom/prometheus

MAINTAINER brian.brazil@robustperception.io


# Add in the configuration file from the local directory.
ADD prometheus.yml /etc/prometheus/prometheus.yml


# Show the link to the consoles by default.
RUN mv /etc/prometheus/consoles/index.html.example /etc/prometheus/consoles/index.html \
  && sed -i 's/index.html.example/index.html/' /etc/prometheus/console_libraries/menu.lib
