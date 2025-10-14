# frontend/Dockerfile
FROM nginx:stable-alpine

# Remove default html
RUN rm -rf /usr/share/nginx/html/*

# Copy the static site
COPY ./Devops_intern.html /usr/share/nginx/html/index.html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
