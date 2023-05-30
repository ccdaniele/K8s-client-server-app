
FROM node:16.15
WORKDIR /Vinology-client
# ENV PATH="/.node_modules/.bin:$PATH"
COPY . . 
RUN apt-get update && apt-get install vim -y
RUN npm install --legacy-peer-deps
CMD ["npm", "start"]

# FROM nginx
# COPY nginx/nginx.conf /etc/nginx/
# EXPOSE 80

# CMD [ "nginx", "-g", "daemon off;" ]

