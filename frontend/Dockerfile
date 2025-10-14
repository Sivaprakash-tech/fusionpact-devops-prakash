FROM nginx:alpine

LABEL maintainer="prakash"
LABEL project="fusionpact-devops"

WORKDIR /usr/share/nginx/html

RUN rm -rf ./*

COPY Devops_Intern.html .

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
