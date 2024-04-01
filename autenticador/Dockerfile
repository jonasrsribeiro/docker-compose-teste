# Use a imagem oficial do Node.js como base
FROM node:latest

# Criação do diretório de trabalho do aplicativo dentro do contêiner
WORKDIR /usr/src/app

# Copiar os arquivos necessários e instalar as dependências
COPY package*.json ./
RUN npm install

# Copiar o código fonte do aplicativo
COPY . .

# Expõe a porta do servidor Express
EXPOSE 5000

# Comando para executar o servidor quando o contêiner for iniciado
CMD ["npm", "start"]