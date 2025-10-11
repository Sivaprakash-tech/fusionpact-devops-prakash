FROM nginx:stable-alpine
WORKDIR /usr/share/nginx/html
# remove default content and copy
RUN rm -rf ./*
COPY Devops_Intern.html ./index.html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
