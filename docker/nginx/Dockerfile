FROM nginx:1.22.0

# Instalación de apps
RUN apt-get update && apt-get install -y \
	bash vim sed

# Configuración de NGINX (agrega el archivo al directorio de nginx)
ADD ./nginx/default.conf /etc/nginx/conf.d/