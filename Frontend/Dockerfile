# Use an official Nginx image as the base image
FROM nginx:latest

# Copy your web application files to the appropriate directory in the container
COPY index.html /usr/share/nginx/html

# Expose the nginx to 8080
EXPOSE 8080

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]

