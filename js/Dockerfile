# Importar Imagenes
FROM node:latest as build_stage
FROM nginx:latest as production_stage
# Si utilizas alguna base de datos como MONGODB debes importar su imagen aqui
FROM mongo:latest

# Configurando el workspace
# - Instalacion de las dependencias en el workdir
WORKDIR /nombre_workdir
COPY package*.json ./

RUN npm install
COPY  . .

# Inicializa la aplicacion > reemplazalo por tu comando de construccion de la app
RUN npm run build

# Inicializa el servidor HTTP para hostear la app
COPY --from=build_stage /nombre_workdir/dist /user/share/nginx/html
EXPOSE 80
CMD [ "nginx", "-g", "daemon off;" ]