FROM mhart/alpine-node:12

ENV NO_UPDATE_NOTIFIER=true
WORKDIR /opt/app-root/src
COPY . .
RUN npm run all:ci && npm run all:build && npm run frontend:purge
EXPOSE 8080
CMD ["npm", "run", "start"]
