# use the nginx image
FROM nginx:latest

# set the working directory in the container
WORKDIR /

# copy the HTML file created before to the nginx default HTML directory
COPY index.html /usr/share/nginx/html

# copy the entrypoint script to the root directory
COPY entrypoint.sh /

# make the entrypoint script executable
RUN chmod +x /entrypoint.sh

# start nginx server
ENTRYPOINT "./entrypoint.sh"