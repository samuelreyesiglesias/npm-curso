![large](https://user-images.githubusercontent.com/51006648/195677745-4b3016e5-3182-4271-a467-c5194ff14bba.png)


# npm-curso
Curso npm - node package manager



npm significa: Node Package Manager
El sitio oficial de npm es: npmjs.com 
en este sitio podemos ver la documentacion oficial.



Node o npm node package manager
Tiene la posibilidad de utilizar modulos
o se pueden crear  y publicar librerias propias.



Para instalar node se debe hacer desde su sitio oficial:
nodejs.org



Existen 2 versiones de node que podemos instalar:
1.) LTS Long Term Support o Soporte a Largo Plazo
2.) CURRENT , es la version mas actual que incluye todos los modulos npm a la fecha de descarga



Descargamos la version que necesitemos
y la intalamos , usualmente en disco c://
en la carpeta programs, si utilizamos windows.



El mismo programa agrega a PATH la ruta
para poder usar npm en las lineas de comando.



Para verificar que se instalo correctamente utilizamos el siguiente comando 
nos sirve para ver la version que hemos instalado de node:
npm -v      



Si deseamos verificar si hay actualizaciones pendientes de version, podemos utilizar el siguiente comando:
npm install -g npm@latest      



Si tu utilizas sistema operativo mac se tiene que descargar npm desde el sitio oficial nodejs.org



El siguiente comando nos sirve para crear archivo package.json 
contiene toda la informacion de nuestro proyecto
npm init      



El siguiente hace lo mismo pero lo hace con valores vacios que posteriormente podemos modificar.
npm init -y
npm init -yes



Los 2 comandos anteriores ambos funcionan o tienen el mismo efecto




Los siguientes datos se deben asignar como lo hacemos en git,
pero mencionar que son datos opciones, no obligatorios:



npm set init.author.email <email>  
npm set init.author.name <name>
npm set init.author.license <MIT>
  
	
	
La importancia de iniciar un proyecto,
cada vez que se crea app.

	
	
Configuracion con datos , importantes

	
	
Crear carpeta del proyecto, por ejemplo para crear un modulo.

	
	

Recapitulando, pasos para iniciar nuestro proyecto:

	
	
0.) Crear directorio
mkdir jsnpm

	
	
1.) Lo primero
git init, sin importar la plataforma
para que viva en un repositorio de forma local

	
	
2.) segundo
	npm init

	
	
Te pide un nombre: (jsnpm)
la version:
descripcion: crear un pack para node
entry point: (index.js)  src/index.js
punto de entrada de nuestro proyecto
test command: pudeen quedar vacios al inicio, son para pruebas
git repository: vacio al comienzo
keywords: javascript,node,package
author: samuel reyes <samuel.reyes@grupolorena.com.sv>
lisence: mit


	
	
Puedes verificar diversas licencias de software en el siguiente enlace:
https://es.wikipedia.org/wiki/Licencia_de_software

	
	
Para abrir un archivo en una carpeta, si tienes
instalado el editor de codigo de visual studio code:
code .

	
	
Pero sino tienes instalado code, puedes abrir el archivo con el editor de
codigo que tu tengas instalado.


	
	

La segunda alternativa para iniciar nuestro proyecto es crear
una configuracion de proyecto vacia:
1.) npm init -y
o npm init -yes

	
	
	
	
Esto nos creara un archivo json con las configuraciones necesarias de nuestro proyecto,
aunque en este caso dejará todos los campos en blanco, para que posteriormente podamos
modificar estos datos.

	
	

Configuracion de datos necesarios para utilizar node., mencionar nuevamente que esto
es opcional, no obligatorio:
  
	
	
npm set init.author.email "s@gmail.com"
npm set init.author.name "samuel"
npm set init.license "MIT"
  
Gracias por leer este documento, ATT. Samuel Reyes, -Software Developer-
