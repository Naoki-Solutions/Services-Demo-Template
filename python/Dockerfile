# Importar Imagenes
FROM python:latest
# Si utilizas alguna base de datos como MONGODB debes importar su imagen aqui
FROM mongo:latest

# Configurando el workspace
WORKDIR /personalized_workspace_directory
COPY . .

RUN apt-get -y update

# En el caso de que ninguna dependencia requiera de instalacion por git
RUN apt-get -y install git 

# Instala las dependencias de tu proyecto
# Si no creaste tu requirements, ve a tu editor donde trabajes y en tu entorno virtual typea:
#   python -m pip freeze > requirements_file.txt
RUN python -m pip install -r requirements_file.txt

# Inicializa la aplicacion > reemplazalo por tu lanzador principal
CMD [ "python", "main_file.py" ]