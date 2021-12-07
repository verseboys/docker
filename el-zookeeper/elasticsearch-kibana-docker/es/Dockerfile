#FROM elasticsearch:6.3.1
FROM docker.elastic.co/elasticsearch/elasticsearch:6.3.1

# x-pack はインストールしない
#```
#ERROR: this distribution of Elasticsearch contains X-Pack by default
#ERROR: Service 'elasticsearch' failed to build: The command '/bin/sh -c elasticsearch-plugin install --batch x-pack' returned a non-zero code: 78
#```
#RUN elasticsearch-plugin install --batch x-pack


ENV VERSION=6.3.1

# https://github.com/medcl/elasticsearch-analysis-ik/releases
ADD https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${VERSION}/elasticsearch-analysis-ik-$VERSION.zip /tmp/
RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install -b file:///tmp/elasticsearch-analysis-ik-$VERSION.zip






# kuromojiをインストール
# RUN elasticsearch-plugin install analysis-kuromoji


RUN rm -rf /tmp/*