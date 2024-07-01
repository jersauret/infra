# Use the official RabbitMQ image from Docker Hub
FROM rabbitmq:3-management

# Enable RabbitMQ plugins
RUN rabbitmq-plugins enable --offline rabbitmq_management

# Expose ports
EXPOSE 15672:15672 5672:5672