Una vez creamos la configuracion inicial de nuestro proyecto nos ubicamos dentro del proyecto, y continuamos:
Aprenderemos a Instalar paquetes globales o locales, la instalacion de dependencias usando npm.


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




npm install moment -save

–save : Este documento que vas a instalar dentro del proyecto es necesario para vivir en producción. Hay que tener cuidado con los paquetes que instalamos, cuando es a producción y cuando no lo es.

–save-dev: Este documento que vamos a instalar solo es necesario en nuestro entorno local o en el de desarrollo. Es importante no mandar dependencias a producción ni omitir algunas que deban de estar en producción.


Listar paquetes instalados de forma global

npm list -g --depth 0


SHORTCUTS
i = install
-S = --save
-D = --save-dev


npm install moment --save : Paquete que se encarga de manejar las fechas en JavaScript
🟢 --save : El documento que vamos a instalar dentro del proyecto es necesario para vivir en produccion.
🟢 -dev : El documento que vamos a instalar solo es necesario en nuestro entorno local o en el entorno de desarrollo
🟢 npm install date-fns : Al igual que moment se engarga de manejar fechas y datos
🟢 npm i : abreviacion de nmp install

🟢 -D : abreviacion para --save-dev


Carpeta node_modules: Aquí es donde se van a instalar los módulos que tú estás agregando a tu proyecto. Esta carpeta es importante para que tu proyecto funcione, pero no debe de ser enviada a ningún repositorio y debemos ignorarla apenas se crea.
Para ignorarla se crea un archivo .gitignore y escribimos: node_modules/
Versión resumida para instalar:



y si requerimos que se registre la versión exacta en el package.json

npm i -D -E moment


El comando que se corre en produccion es:

npm install --only=prod
# or
npm install --only=production



npm install moment: Instalar dependencia.
npm install moment --save: La dependencia instalada es necesaria para vivir en producción.
npm install moment --save-dev: La dependencia solo es necesaria en el entorno local o de desarrollo.
npm i date-fns -D: Instalar como dependencia de desarrollo.
npm i moment -S: Instalar dependencia necesaria para producción.
sudo npm install -g nodemon: Instalar dependencia de forma global.
npm list -g --depth 0: Listar dependencias instaladas de forma global.


También se puede usar NPX para no instalar módulos globalmente:
npm install nodemon -D
npx nodemon





INSTALAR react

npm install react --dry-run



INSTALAR USANDO FORCE

npm install webpack -f
npm install webpack -force

luego de instalar webpack se lleva a devdependencies.

npm install sirve para volver a crear
o instalar las dependencias especificadas en
package json.



npm i json-server@0.15.0

esto es para cuando tenemos versiones especificas antiguas que tenemos que instalar.


npm list       listar 






npm outdate         me muestra paquetes desactualizados



npm outdate --dd   , cualquier comando que quieras ver detallado


npm update        , actualizar paquetes a la ultima version


actualizar a la ultima version
npm install json-server@latest


Como desintar paquete
npm uninstall json-server



desintalar dependencia pero sin eliminarlo de package json

npm uninstall webpack --no-save



Un pequeño resumen:

Actualizar paquetes

Revisar que paquetes disponen de nuevas versiones
npm outdate

Para ver un output más detallado
npm outdate --dd

Actualizar los paquetes que no están en la ultima versión
npm update

Actualizar un paquete especifico
npm install json-server@latest

Eliminar paquetes

Eliminar un paquete de node_modules y del archivo package.json
npm uninstall json-server

Desinstalar un paquete de todo node_modules pero no del archivo package.json
npm uninstall webpack --no-save
