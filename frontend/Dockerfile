# Use an official node runtime as a parent image
FROM node:10

WORKDIR /app/

# Installing dependencies
COPY package*.json ./
RUN npm install
 
# Add rest of the client code
COPY . /app/

# Building app
RUN npm run build

EXPOSE 3000

# CMD npm start
CMD [ "npm", "run", "dev" ]
