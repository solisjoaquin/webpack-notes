# webpack-notes

Webpack es un empaquetador de modulos para aplicaciones modernas en JS

![webpack](https://raw.githubusercontent.com/solisjoaquin/webpack-notes/main/webpack.png)

Los archivos de la izquierda pasan a ser los de la derecha.

# Iniciar un proyecto 

Requisitos

```
node
```

Crear carpeta **webpack-4**

```
mkdir webpack-4
cd webpack-4
npm init  -y
```
Instalar webpack

```
npm i webpack --save-dev
```
Instalar webpack CLI

```
npm i webpack-cli --save-dev
```
Webpack necesita del CLI para ejecutar sus comandos.

Creamos un archivo index.js con un simple console.log
```
console.log("Hello world)
```

Para crear un archivo con webpack del archivo index.js, usamos el siguiente comando:
```
npx i webpack --entry ./index.js --output ./bundle.js
```

Esto nos creará un archivo llamado bundle.js que si lo abrimos nos mostrará el console.log del index.js pero con mas configuraciones y todo en una sola linea. Esto es porque lo creamos para producción.

Para crearlo en modo desarrollo podemos usar el comando 
```
npx i webpack --entry ./index.js --output ./bundle.js --mode development
```
Ahora el bundle.js esta escrito en muchas lineas.

