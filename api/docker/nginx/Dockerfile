#Descarga la img nginx:1.19
FROM nginx:1.19

#Se define el argumento UID y se expone
ARG UID
EXPOSE $UID

#Añade un usuario dentro del contenedor con el nombre appuser
RUN adduser -u ${UID} --disabled-password --gecos "" appuser

#Copia la configuracion del fichero default.config al fichero conf.d
COPY default.config /etc/nginx/conf.d