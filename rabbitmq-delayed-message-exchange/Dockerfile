FROM rabbitmq:3.8.9-management
MAINTAINER  JeffBRIAN
COPY  rabbitmq_delayed_message_exchange-3.8.0.ez   /plugins
RUN rabbitmq-plugins enable --offline rabbitmq_delayed_message_exchange
