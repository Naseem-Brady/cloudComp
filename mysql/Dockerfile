# Use mysql/mysql-server:latest as the base image
FROM mysql/mysql-server:latest

# Set environment variables
ENV MYSQL_ROOT_PASSWORD=pass

# Copies cattle.csv file to docker image?
COPY cattle.csv /image

# Expose port to allow connections from outside the Docker node
EXPOSE 3306
