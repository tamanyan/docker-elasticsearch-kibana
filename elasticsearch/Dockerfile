FROM docker.elastic.co/elasticsearch/elasticsearch:6.2.3
USER root

ADD config/elasticsearch.yml /usr/share/elasticsearch/config/
RUN chown elasticsearch:elasticsearch config/elasticsearch.yml

RUN cd /usr/share/elasticsearch
RUN bin/elasticsearch-plugin install analysis-kuromoji
RUN bin/elasticsearch-plugin install analysis-icu

USER elasticsearch