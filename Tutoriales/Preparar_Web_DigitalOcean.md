---
layout: post
title: Web con DigitalOcean
export_on_save:
  html: true
---

# Cómo preparar una página web usando DigitalOcean.com y Name.com
[TOC]

# Licencias de Software de la UCM

A los estudiantes de la Complutense, aunque parezca que no, nos dan muchas ayudas de software, pero nadie nos explica cuáles o cómo usarlas.
Lo primero de lo que me enteré fue de las licencias de Microsoft y de MatLab que nos ofrecían.
También nos ofrecen licencias de Adobe para programas como Photoshop. Creo que es para versiones viejas pero siguen siendo un buen comienzo al mundo del diseño.
Lo que más útil me ha sido es el Google Drive casi ilimitado en la cuenta de correo que nos proporciona la universidad. Sólo hay que acceder a la web de Drive desde esa cuenta.

Para más información sobre todo esto, consulta la [web oficial de la UCM](https://ssii.ucm.es/software-ucm) o pregúntame.

## Github Student Developer Pack

Lo último de lo que he sido consciente, y relevante para este post, es el [Github Student Developer Pack](https://education.github.com/pack/offers).

Si ya tienes GitHub en otro email,

Al parecer

# Preparación

## Preparando un servidor en DigitalOcean

## Preparando un dominio en Name

# Nuestra primera página

## HTML y Markdown

Como sabreis, HTML es el lenguaje de las páginas web. Menos conocido es Markdown, un [lenguaje de marcado] que permite transformar texto plano en código HTML o .tex (usando [Pandoc], es algo más avanzado) de una forma sencilla y rápida.

Lo bueno de markdown es que es compatible con ecuaciones de LaTeX. Así, podemos escribir directamente

```latex

```

y tendremos la ecuación debidamente renderizada:

$$
a
$$

Si quereis aprender más sobre Markdown y cómo funciona con LaTeX, empezad por la [página oficial], y sabed que para el renderizado se suele usar unos motores de LaTeX online, normalmente [MathJax] o [KaTeX].

Hay montones de editores que soportan markdown, tanto en la web como para instalar.
Nos centraremos en dos:

- El editor de texto [Atom]
- El editor online de markdown [Stackedit]

### Preparando una página de inicio con Stackedit

### Preparando una página de inicio con Markdown Preview Enhanced

### Añadiendo imágenes

## Exportando y subiendo a la web con un programa de FTP

### Windows

### Mac

### Linux
Os buscais la vida, ya sabreis como va la vaina. Si conoces un buen software de FTP, dimelo y lo añadiré aquí.

# Conclusiones

Se quedan muchas cosas en el tintero, aunque con esto ya podrías hacerte un blog sencillito o empezar a cacharrear con HTML. Recomiendo los [Cursos de Formación Informática](https://www.ucm.es/estudios/grado-cficompetencias) de la propia UCM.

## En el futuro

En futuros posts, me gustaría comentar...

- [ ] Un problema al usar este método es que no aparece ninguna barra o icono en la parte superior de la página para ir otra vez a nuestra web principal. Yo lo he resuelto añadiendo a mano un poco de HTML. Esto puede resolverse añadiendo enlaces de markdown en alguna parte de la página que lleven al resto de la web, pero es un método poco satisfactorio. A ver como se puede resolver.

- [ ] Mejorar las seguridad de nuestra web usando https.
Para que no salga el aviso en la barra de direcciones.

![Aviso](img/aviso_seguridad.gif)

- [ ] Preparar Jekyll y CSS en nuestro proyecto para simplificar el proceso de subida de archivos.

- [ ] Una mejor introducción a Markdown y YAML para bloguear como un hacker. Por ahora [este post](https://agea.github.io/tutorial.md/) es el mejor que he encotrado.

- [ ] Profundizar más en Atom y cómo sincronizar tus plugins y snippets entre ordenadores. De hecho, hay mucho que comentar en cuanto a snippets y extensiones de Atom.

- [ ] Añadir plantillas de HTML chulas [como estas](https://onepagelove.com/templates/html-templates) y estilos de Wordpress y Blogspot.

- [ ] Este tutorial es para hacer una web, pero el servidor que hemos montado en DigitalOcean puede usarse para muchas otras cosas. Me gustaría comentar cómo montar tu propio servidor de Git para proyectos que no quieras subir a GitHub o a GitLab.
