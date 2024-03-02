# Use mysql/mysql-server:latest as the base image
FROM mysql/mysql-server:latest

# Set environment variables
ENV MYSQL_ROOT_PASSWORD=root_password

# Copy external CSV file into the image
COPY cattle_data.csv /tmp/cattle_data.csv

# Create database and table during initialization
COPY init.sql /docker-entrypoint-initdb.d/init.sql

# Expose port to allow connections from outside the Docker node
EXPOSE 3306
