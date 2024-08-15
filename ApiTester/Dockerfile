# Usa una imagen base adecuada para Node.js
FROM node:14

# Establece el directorio de trabajo
WORKDIR /usr/src/app

# Copia el archivo package.json y package-lock.json
COPY package*.json ./

# Instala las dependencias
RUN npm install

# Copia el resto del c贸digo de la aplicaci贸n
COPY . .

# Expone el puerto en el que la aplicaci贸n se ejecuta
EXPOSE 8000  
# Comando para iniciar la aplicaci贸n
CMD ["npm", "start"]