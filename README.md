#Paquete DEB vx-dga-l-google-chrome-extesions
Paquete que despliega de forma desatendida y para todos los usuarios de la máquina las extensiones requeridas por el centro.
La selección de las extensiones se realizará por las etiquetas de centro asignadas en el equipo.

# Usuarios Destinatarios

Centros que desean tener instaladas ciertas extensiones en todos los equipos del centro (o en aquellos que determinen)

# Aspectos Interesantes:
```
Google Chrome deberá estar instalado y se requerirá su instalación en el caso de no estar.
```
# Como Crear el paquete DEB a partir del codigo de GitHub
Para crear el paquete DEB será necesario encontrarse dentro del directorio donde localizan los directorios que componen el paquete.  Una vez allí, se ejecutará el siguiente comando (es necesario tener instalados los paquetes apt-get install debhelper devscripts):

```
apt-get install debhelper devscripts
/usr/bin/debuild --no-tgz-check -us -uc
```

# Como Instalar el paquete generado vx-dga-l-*.deb:
Para la instalación de paquetes que estan en el equipo local puede hacerse uso de ***dpkg*** o de ***gdebi***, siendo este último el más aconsejado para que se instalen también las dependencias correspondientes.
```
gdebi vx-dga-l-*.deb
```
