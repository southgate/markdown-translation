De: https://github.com/facebook/chef-cookbooks/edit/master/CONTRIBUTING.md

# Contribuir a los libros de cocina del chef de Facebook

## Rebaja de prueba

Aquí hay un  ~~par de algunas pruebas~~ de Markdown con sabor a GitHub de @southgate.

:entonces: | :ok_hand: | :fruncir el ceño: |
---------|----------|----------|
Enormes felicitaciones  | Menos felicitaciones | Sin felicitaciones

- [ ] Tarea 1
- [ ] Tarea 2
- [ ] Tarea 3

## Nuestro proceso de desarrollo
Este repositorio se sincroniza desde un repositorio interno. Aceptamos absolutamente tirar
solicitudes y se ocupará de la fusión apropiadamente.

Utilizamos Foodcritic para las pruebas de corrección de Chef y Rubocop para el estilo Ruby
linting. Nuestros conjuntos de reglas se sincronizan interna y externamente para garantizar
calidad y estilo de código consistentes para todos.

## Acuerdo de licencia de colaborador ("CLA")
Para aceptar su solicitud de extracción, necesitamos que envíe un CLA. Sólo necesitas
para hacer esto una vez para trabajar en cualquiera de los proyectos de código abierto de Facebook.

Complete su CLA aquí: <https://code.facebook.com/cla>

## Requisitos previos
En primer lugar, gracias por su interés en contribuir, ¡damos la bienvenida a las solicitudes de extracción!

Antes de enviar una solicitud de extracción a este repositorio es importante recordar que el
Las API basadas en atributos aquí son un modelo muy diferente al de otras comunidades
Cocina. Para construir ese modelo, hay una forma específica en que los libros de cocina necesitan
para ser escrito.

Le recomendamos encarecidamente que se asegure de leer el [README.md](README.md)
[Philosphy.md](https://github.com/facebook/chef-utils/blob/master/Philosophy.md).
También le recomendamos que haya configurado un entorno que utilice nuestro orden de lista de ejecución
(libros de cocina principales primero, todo lo demás después).

Por último, asegúrese de seguir el enfoque de 3 fases:

 * `attributes/` los archivos configuran una API y nunca tocan los atributos de otro libro de recetas.
 * `recipes/` recursos de configuración de archivos (como plantillas o servicios) y
   API (lectura: establecer atributos para otros libros de recetas)
 * Los atributos solo se consumen en (también `runtime`conocido como  `converge time`).
   Algunos ejemplos son  `templates`,  `ruby_blocks`,  `whyrun_safe_ruby_blocks`o
   `providers`.

## cuestiones
Usamos problemas de GitHub para realizar un seguimiento de errores públicos. Por favor, asegúrese de que su descripción es
claro y tiene instrucciones suficientes para poder reproducir el problema.

Facebook tiene un [programa de recompensas](https://www.facebook.com/whitehat/)for the safe
divulgación de errores de seguridad. En esos casos, por favor pase por el proceso
descrito en esa página y no presentar un problema público.

## Envío de una solicitud de extracción

¿Tienes una solución o función? ¡impresionante! Cuando envíe la solicitud de extracción le sugerimos que
incluir parte de la salida de una ejecución de chef aplicable.

Si se trata de una nueva API (atributo), asegúrese de que está documentada
libro de cocina LÉAME.

Realizaremos todas las contribuciones a los mismos estándares de calidad y estilo que el
código existente.


### Nuevos libros de cocina

Nos gustaría mantener este repositorio centrado en libros de cocina "básicos" que administran la base
Nso Si desea contribuir con un libro de cocina de este tipo, le recomendamos que comience por
presentar un problema primero para evitar duplicar el esfuerzo (podemos tener uno que podemos
tratar de código abierto, u otras personas pueden estar escribiendo uno) antes de trabajar en él.

Si quieres aportar un libro de cocina que no caiga en esa categoría (por ejemplo.
la gestión de cosas de escritorio u otros servicios), entonces le sugerimos que nos señale a un
en un repositorio donde le gustaría mantenerlo y estaremos encantados de revisarlo y agregar un
puntero a su repo en nuestro 
[UNIVERSE.md](https://github.com/facebook/chef-cookbooks/blob/master/UNIVERSE.md)
archivo.

Usamos el `fb_`prefijo para denotar libros de cocina que se ajusten
este modelo y vienen de este repositorio, pero no dude en publicar libros de cocina en otros lugares
que dejan este modelo y utilizan otros prefijos.

## licencia
Al contribuir a este repositorio, usted acepta que sus contribuciones serán
licencia bajo su licencia Apache 2.0.
