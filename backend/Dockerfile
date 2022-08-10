FROM node:14.19.3-buster

WORKDIR /app

COPY package.json package.json 
COPY package-lock.json package-lock.json 

RUN npm install next react react-dom

COPY . .

RUN npm run build

RUN npm ci --production

#CMD ["npm", "run", "start"]
