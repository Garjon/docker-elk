FROM kibana:latest

RUN apt-get update && apt-get install -y netcat

COPY entrypoint.sh /tmp/entrypoint.sh
RUN chmod +x /tmp/entrypoint.sh

# Sense is a developer portal for writing queries against Kibana
# RUN kibana plugin --install elastic/sense

CMD ["/tmp/entrypoint.sh"]
