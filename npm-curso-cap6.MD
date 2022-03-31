

npm install           paquetes instalados
npm audit             auditar

npm update eslint-utils --depth 2                   para actualizar el paquete pero tambien las dependencias
npm audit           emcpmtrar vulnerabilidades
npm audit --json        generar un archivo formato json con los datos


En bin la ruta es la siguiente:
#!/usr/bin/env node

El name del proyecto en el package.json, y la propiedad contenida en la propiedad bin,
tambien deben coincidir. Significa esto:

{
    "name": "module-1-sri",
    "version": "1.0.2",
    "description": "",
    "main": "src/index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [
        "js"
    ],
    "author": "samuel reyes <samuelreyesiglesias@gmail.com>",
    "license": "MIT",
    "prefferGlobal": true,
    "bin": {
        "module-1-sri": "./bin/global.js"
    },
    "publishConfig": {
        "access": "public"
    }
}


Para chequear funciones:
node bin/global.js





Agregar a un repositorio vaciio un proyecto:
git remote add origin https:github.com/samuelreyesiglesias/module-1-sri.git
 
$ git add .
  
$ git commit -m 'module 1 ' 
  
$ git push -u origin master 
 

 DESPUES DE CREAR EL REPOSITORIO, EJECUTAMOS NUEVAMENTE:
 git init


 PARA QUE NOS ACTUALICE LOS DATOS DE NUESSTRO REPOSITORIO,
 por ejemplo nos agrega repository, bugs, homepage,

 {
  "name": "module-1-sri",
  "version": "1.0.2",
  "description": "Whenever I start a new project, I don't know what to write for the first commit. After doing a “git init” there is technically nothing there...",
  "main": "src/index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [
    "js"
  ],
  "author": "samuel reyes <samuelreyesiglesias@gmail.com>",
  "license": "MIT",
  "prefferGlobal": true,
  "bin": {
    "module-1-sri": "bin/global.js"
  },
  "publishConfig": {
    "access": "public"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/samuelreyesiglesias/module-1-sri.git"
  },
  "bugs": {
    "url": "https://github.com/samuelreyesiglesias/module-1-sri/issues"
  },
  "homepage": "https://github.com/samuelreyesiglesias/module-1-sri#readme"
}

