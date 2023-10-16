FROM node:16-alpine
EXPOSE 3001
WORKDIR /app/back-end
COPY package*.json ./
RUN npm clean-install
ADD node_modules.tar.gz .
COPY . .
ENTRYPOINT [ "npm" ]
CMD [ "start" ]