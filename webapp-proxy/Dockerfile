# Use an official NGINX image as a base
FROM nginx:latest

# Copy the nginx configuration file
COPY nginx.conf /etc/nginx/nginx.conf

# Remove the default.conf file to avoid conflicts
RUN rm /etc/nginx/conf.d/default.conf

# Expose the port for the reverse proxy
EXPOSE 80

# Run NGINX when the container starts
CMD ["nginx", "-g", "daemon off;"]