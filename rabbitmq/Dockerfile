FROM rabbitmq:3.5.3

COPY rabbitmq_auth_backend_http-3.5.x-0.ez /usr/lib/rabbitmq/lib/rabbitmq_server-3.5.3/plugins/rabbitmq_auth_backend_http-3.5.x-0.ez
#COPY rabbitmq.config /etc/rabbitmq/rabbitmq.config

RUN rabbitmq-plugins enable --offline rabbitmq_management
RUN rabbitmq-plugins enable --offline rabbitmq_management_visualiser
RUN rabbitmq-plugins enable --offline rabbitmq_auth_backend_http
RUN rabbitmq-plugins enable --offline rabbitmq_stomp
RUN rabbitmq-plugins enable --offline rabbitmq_web_stomp

EXPOSE 15671 15672 15674
