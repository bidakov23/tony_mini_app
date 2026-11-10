FROM node:24-bookworm-slim
WORKDIR /app
COPY package.json server.js ./
COPY public ./public
RUN mkdir -p /app/data && chown node:node /app/data
USER node
EXPOSE 3000
CMD ["node", "server.js"]
