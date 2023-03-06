FROM node:latest

WORKDIR /gluestack/{INSTANCE_NAME}

COPY package*.json ./
COPY app.json ./
COPY . ./

RUN npm install -g expo-cli

EXPOSE 19000

RUN ["npm", "install", "-f"]

# Run the app
CMD ["sh", "-c", "npm run start"]
