FROM node:10-alpine
RUN mkdir -p /home/node/Angular6/node_modules && chown -R node:node /home/node/Angular6
WORKDIR /home/node/Angular6
COPY . ./
RUN ls -ltra 
USER node
RUN npm install
COPY --chown=node:node . .
EXPOSE 4200
CMD [ "npm", "start" ]
