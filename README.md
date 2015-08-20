Keep in Memory
==============

Este es un fork de [My Personal Kanban](https://github.com/greggigon/my-personal-kanban), una pequeña aplicación para gestión de proyectos según el modelo kanban escrita por Greg Gigon. Está escrita en javascript y tiene funcionalidades muy básicas.

## Functionalidades

Kim es un gestor de proyectos que sigue el método kanban y es el equivalente digital de una pizarra kanban. Se ejecuta en el navegador sin necesidad de bases de datos, pues estos se guardan en el navegador mediante el almacenamiento local.

Con KiM podrás hacer lo siguiente:
- Crear y borrar proyectos
- Crear y gestionar columnas
- Crear y gestionar tarjetas
- Asignar colores según la prioridad a cada tarjeta
- Mover las tarjetas entre columnas
- Archivar las tarjetas
- Exportar e importar los proyectos

## Descarga



## Instalación

Descarga el paquete, descomprímelo y abre el `index.html` en cualquier navegador. También puedes colocar la carpeta descomprimida en la raiz de tu servidor local o subirla a un servidor remoto.

## Temas

Los temas son sencillamente archivos __CSS__ acompañados de una imagen, que sobreescriben los estilos básicos. __KiM__ viene con un único tema pero se pueden instalar más de forma muy sencilla y podremos seleccionarlos desde el menú de la aplicación.

### Crear un tema
La forma más sencilla de crear un tema nuevo es copiar y renombrar el archivo `default.css` de la carpeta __styles/themes__ y aplicar los cambios directamente en la hoja de estilos. 

Una vez hecho esto, debemos acompañar el tema de un pantallazo que colocaremos en la carpeta __img/themes__. Despues registraremos el nuevo tema añadiendo una nueva linea en el archivo __scripts/themes.js__ file. 

```
window.themes = [
	{"name": "Default", "css":"default"},
	{"name": "Tu Nuevo Tema", "css":"tu-nuevo-tema"}
];
```

> El nombre del archivo de imagen debe ser el mismo que el del valor del atributo `css` en __themes.js__

## TODO

En un futuro me propongo conseguir lo siguiente:
- Añadir más temas
- Sustituir Bootstrap por Materialize
- Adaptarla para dispositivos móviles
- Empaquetarla para escritorio, usando appjs o similar
- Crear app para Android?
