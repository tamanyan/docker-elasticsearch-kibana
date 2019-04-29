FROM docker.elastic.co/kibana/kibana:6.2.3
USER root

RUN bin/elasticsearch-plugin install analysis-kuromoji

USER elasticsearch