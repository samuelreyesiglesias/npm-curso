PASOS
0 MKDIR NAMEPROJECT
1 GIT INIT
2 NPM INIT
3 MKDIR SRC
4 MKDIR BIN
5 CREAR ARCHIVO INDEX.JS EN SRC
6 CREAR ARCHIVO GLOBAL.JS EN BIN
7 AGREGAR LINEAS en el package json
{
    "name": "test",
    "version": "1.0.0",
    "description": "test",
    "main": "src/index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [
        "js",
        "test"
    ],
    "bin": {
        "test": "./bin/global.js"
    },
    "prefferGlobal": true,
    "author": "samuel reyes <samuelreyesiglesias@gmail.com>",
    "license": "MIT",
    "publishConfig": {
        "access": "public"
    }

}

O ASI:

{
    "name": "random-messages-sri",
    "version": "1.0.0",
    "description": "random de mensajes",
    "main": "src/index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [
        "javascript",
        "node",
        "npm"
    ],
    "author": "samuel reyes <samuel.reyes@grupolorena.com.sv>",
    "license": "MIT",
    "bin": {
        "random-msg": "./bin/global.js"
    },
    "prefferGlobal": true,
    "dependencies": {
        "user": "^0.0.0"
    },
    "publishConfig": {
        "registry": "https://registry.npmjs.org/"
    }
}


8 AGREGAR DENTRO DEL ARCHIVO GLOBAL.JS
el REQUIRE Y LLAMADO A LA FUNCION

#!/usr/bin/env node

let random = require("../src/index.js");

random.randomMsg();



9 EN EL ARCHIVO INDEX.JS
AGREGAR LA FUNCION Y EXPORTARLA COMO MODULO.

const messages = ["Samuel", "Santiago", "Alexander", "Glenda"];

const randomMsg = () => {
    const message = messages[Math.floor(Math.random() * messages.length)];
    //return message;
    console.log(message);
}

module.exports = { randomMsg };


10: EJECUTAR EL COMANDO 
NPM LINK


11: LOGUEARSE
NPM LOGIN
O
NPM ADDUSER

12: EJECUTAR EL COMANDO 
NPM PUBLISH --ACCESS=PUBLIC


LISTO
