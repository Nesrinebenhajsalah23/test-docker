FROM node:18
WORKDIR /app
COPY package*.json ./
ENV NODE_OPTIONS="--max-old-space-size=512"
RUN npm install --jobs=1 --legacy-peer-deps
COPY . .
EXPOSE 3001
CMD ["node", "server.js"]

