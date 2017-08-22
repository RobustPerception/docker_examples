FROM java:8

RUN mkdir /opt/jmx_prometheus_httpserver && wget 'http://central.maven.org/maven2/io/prometheus/jmx/jmx_prometheus_httpserver/0.9/jmx_prometheus_httpserver-0.9-jar-with-dependencies.jar' -O /opt/jmx_prometheus_httpserver/jmx_prometheus_httpserver.jar

COPY entrypoint.sh /opt/entrypoint.sh
ENTRYPOINT ["/opt/entrypoint.sh"]
