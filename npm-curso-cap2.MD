
Una vez creamos la configuracion inicial de nuestro proyecto nos ubicamos dentro del proyecto, y continuamos:
Aprenderemos a Instalar paquete global o local,
instalacion de dependencias


Crear directorio:
mkdir src

Cambiar a ese directorio:
cd src

Crear archivo:
touch index.js        en mac y linux
echo >> index.html    en windows 

Ver directorio actual, print working directory, cuya traducción sería imprimir directorio de trabajo:
pwd           

Instalacion de Recursos:
npm install es el comando necesario para instalar recursos o paquetes

en este ejemplo tenemos el nombre de uno en especifico para fechas:
moment

El comando completo es:
npm install moment --save        para el manejo de fechas, se instala como una dependencia,

--save sirve para especfiicar que es necesario que viva en produccion

npm install moment --save-dev
--save-dev solo es necesario en nuestro entorno local.

Archivo git ignore es para que git ignore archivos
.gitignore

y dentro del archivo especificmamos que esta carpeta sea ignorada de la siguiente manera:
node_modules/

En el archivo package.json se agrega en la propiedad de jsons: moment


descargar otro paquete para manejar fechas: 
npm install date-fns --save--dev


npm i date-fns -

npm i date-fns -S
npm i moment -S


Nodemon es para que este escchando:
npm install -g nodemon

con permisos de administrador en windows
y en linux usar sudo y mac

una vez instalado.
comando para ver si esta instalado

npm list -g --depth 0

Instalar de forma opcional el siguiente ...

npm install eslint -O

npm fund  que puede ser apoyado o recibe donaciones
