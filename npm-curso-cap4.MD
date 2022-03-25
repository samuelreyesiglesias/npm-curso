VERSIONAMIENTO 

CAMBIOS MAYORES
MENORES ^
PATCH ~

CARET  ^
PARA CAMBIOS MENORES O PARCHES

TILDE ~
PARCHES(BUG FIXES)


UNA TILDE ESTABLE QUE SOLO VAMOS A HACER CAMBIOS O 
ACTUALIZACIONES DE FIXES

SIQUEREMOS GARANTIZAR QUE NOS VAMOS A QUEDAR EN CIERTA
VERSION SE ELIMINA EL CARET ^

Además de esos símbolos, también tenemos:

< : Versión menor a la indicada.
<= : Versión menor o igual a la indicada.
> : Versión mayor a la indicada.
>= : Versión mayor o igual a la indicada.
Los cuales se utilizan así:

"dependencies": {
    "json-server": ">0.15.1",
    "moment": ">=2.26.0",
    "date-fns": "<2.14.0",
     "react": "<=16.12.0"
}

^ = Si mantenemos el caret dentro de la configuración de nuestro package estamos garantizando que cuando realicemos una actualización o tengamos un cambio que podamos realizar, vamos a hacer actualización de los cambios menores y de los parches o bug fixes.
Para quedarnos en una sola versión eliminamos el caret.

~ = Establece que vamos a recibir actualizaciones o cambios solamente de los cambios que son parches o bug fixes.


^ Acento circunflejo
~ Virgulilla



Scripts dentro de package.json



Scripts: comandos que podemos ejecutar desde la consola. nos dan una serie de salidas los scripts


build: webpack --mode production
start:webpack --
format: "prettier --write 

"hola": "node",
"deploy":"npm run format ; npm run build";


npm i -g serve              instalar de manera global server
serve .                    levantar el servidor


