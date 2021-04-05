FROM node:alpine

# Add the following line 
ENV CI=true

WORKDIR /app
COPY package.json ./
RUN npm install
RUN npm audit fix --force
COPY ./ ./

CMD ["npm", "start"]