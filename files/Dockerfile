# Dockerfile

# Base image
FROM ubuntu:latest

# Update package list and install apache2 and MariaDB
RUN apt update && \
    apt install -y apache2 mariadb-server && \
    apt clean

# Expose the web and MariaDB ports
EXPOSE 80 3306

# Start Apache2 and MariaDB services
CMD service apache2 start && service mariadb start && tail -f /dev/null
