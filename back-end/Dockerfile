FROM node:16

# diretório criado no container
WORKDIR /usr/src/

# copies our package.json and installs it
COPY package*.json ./ 

# copia todos os arquivos para o container
COPY . . 

RUN npm i 
RUN npm run build

EXPOSE 5000

CMD [ "npm", "start" ]