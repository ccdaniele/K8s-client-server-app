# =v1.2.0 - Updating react env vars: REACT_APP_API_ENDPOINT=SERVERSVC_SERVICE_HOST 
#         - Adding VIM
FROM node:16.15
WORKDIR /Vinology-client
# ENV PATH="/.node_modules/.bin:$PATH"
COPY . . 
RUN apt-get update \
    && apt-get install -y \
        nmap \
        vim

RUN npm install --legacy-peer-deps
CMD ["npm", "start"]


