FROM node:16-alpine
EXPOSE 3000
WORKDIR /app/front-end
COPY package*.json ./
RUN npm install
ADD node_modules.tar.gz .
COPY . .
ENTRYPOINT [ "npm" ]
CMD [ "start" ]
