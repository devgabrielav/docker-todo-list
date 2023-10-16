FROM betrybe/puppetter:1.0
WORKDIR /app/tests
COPY package*.json ./
RUN npm clean-install
ADD node_modules.tar.gz .
COPY . .
ENTRYPOINT [ "npm" ]
CMD [ "test" ]