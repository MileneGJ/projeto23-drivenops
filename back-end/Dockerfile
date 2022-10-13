FROM node:16 as base

# diretório criado no container
WORKDIR /usr/src/

# copies our package.json and installs it
COPY package*.json ./ 

RUN npm i 

# copia todos os arquivos para o container
COPY . . 

FROM base as production

RUN npm run build