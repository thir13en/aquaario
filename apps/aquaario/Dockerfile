FROM node:lts-alpine
WORKDIR /app
COPY ./dist/apps/api .
COPY ./apps/api/package.json .
ENV NODE_ENV=production
ENV PORT=3333
EXPOSE ${PORT}
RUN npm install --production --silent
CMD node ./main.js
