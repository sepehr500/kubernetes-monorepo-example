FROM node:8
WORKDIR /app
COPY package.json .
COPY package-lock.json .
RUN npm install --production
RUN apt install lsof
COPY . .
EXPOSE 8080
CMD [ "npm", "start" ]