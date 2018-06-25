# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch-oss:6.3.0

COPY readonlyrest-1.16.21_es6.3.0.zip .

COPY config/readonlyrest.yml  /usr/share/elasticsearch/config/readonlyrest.yml
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
RUN pwd
RUN elasticsearch-plugin install --batch file:///usr/share/elasticsearch/readonlyrest-1.16.21_es6.3.0.zip
