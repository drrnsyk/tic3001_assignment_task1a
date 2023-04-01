FROM nginx:latest

# Copy custom Nginx configuration file to the container
COPY nginx.conf /etc/nginx/nginx.conf
COPY mynodeapp.conf /etc/nginx/mynodeapp.conf

# Copy website files to the container
COPY index.html /etc/nginx/html/

# Expose port 80 to the host
EXPOSE 80

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]