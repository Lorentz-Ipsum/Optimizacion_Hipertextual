---
layout: post
title: Web con DigitalOcean
export_on_save:
  html: true
---

# Cómo preparar una página web usando DigitalOcean.com y Name.com
[TOC]

# 0. Licencias de Software de la UCM

A los estudiantes de la Complutense, aunque parezca que no, nos dan muchas ayudas de software, pero nadie nos explica cuáles o cómo usarlas.
Lo primero de lo que me enteré fue de las licencias de Microsoft y de MatLab que nos ofrecían.
También nos ofrecen licencias de Adobe para programas como Photoshop. Creo que es para versiones viejas pero siguen siendo un buen comienzo al mundo del diseño.
Lo que más útil me ha sido es el Google Drive casi ilimitado en la cuenta de correo que nos proporciona la universidad. Sólo hay que acceder a la web de Drive desde esa cuenta.

Para más información sobre todo esto, consulta la [web oficial de la UCM](https://ssii.ucm.es/software-ucm) o pregúntame.

## Github Student Developer Pack

Lo último de lo que he sido consciente, y relevante para este post, es el [Github Student Developer Pack](https://education.github.com/pack/offers).
Básicamente es un conjunto de licencias y promociones que nos ofrecen diversas empresas tecnológicas. Vamos a usar la de DigitalOcean.com y la de Name.com (o NameDomain.com) para crear nuestra web.

> Lo primero que necesitas es una cuenta en GitHub.com.
> Si quieres usar el mail de la UCM es sencillo. Tan sólo registrate.
> Si vas a usar otra cuenta de correo o ya tienes GitHub, no hay problema. Puedes conseguir los beneficios de tu cuenta UCM.

> Con tu cuenta iniciada, ve a https://education.github.com/students y sigue los pasos.

> Una vez registrado, en https://education.github.com/pack/offers podrás ver todas las ofertas.
> Aquí es donde tendrás que buscar DigitalOcean y Name.com para acceder a sus webs y canjear tus licencias.

---
# 1. Preparación

## Preparando un servidor en DigitalOcean

Sé que es algo cutre, pero por ahora simplemente voy a pegar aquí este video

[![](http://img.youtube.com/vi/cMD6_MwgHDo/0.jpg)](http://www.youtube.com/watch?v=cMD6_MwgHDo "")

en el que vienen todos los pasos:

1. Desde la cuenta de DigitalOcean, crear un Droplet de Ubuntu(o si quiers, de Wordpress[^wordpress]).
2. Auntenticarlo y acceder desde una terminal usando SSH.
3. Cambiar la contraseña.
4. Instalar nginx[^nginx] en nuestro servidor.
5. Asociar un dominio (para este paso necesitaremos haberlo creado, en la siguiente sección).

Siguiendo los pasos tendréis vuestro servidor a punto.

Si prefieres leer, [en este post](https://www.digitalocean.com/docs/droplets/how-to/create/) está explicado lo mismo más o menos hasta el punto 2.
Para instalar **nginx**, [en este post lo explican](https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-18-04). También viene cómo crear un firewall para mejorar la seguridad, pero no es necesario.

Si aún tienes ganas de más, [aquí explican más cosas que hacer con tu servidor](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-16-04) como crear otros usuarios con sus propias contraseñas y permisos (aumenta la seguridad), o crear un firewall (otra vez).

[^wordpress]: Si sólo quieres bloguear, puedes crear un server con Wordpress directamente, pero búscate la vida. Quizá algo de este post te sea útil. Y si no seguramente haga un post sobre eso algún día.
[^nginx]: Nginx es el programa que "servirá" las páginas web que tengamos en nuestro servidor cuando alguien acceda a través de un navegador.

## Preparando un dominio en Name

Sólo hay que seguir los pasos. Recuerdo que había alguna dificultad en cierto punto pero nada imposible de resolver.
Extenderé este punto algún día, con las dificultades que haya.

## Asociando el nombre del dominio con el servidor

El video de arriba explica todos los pasos.
[Este enlace me resolvió los problemas que me encontré.](https://www.digitalocean.com/community/tutorials/how-to-point-to-digitalocean-nameservers-from-common-domain-registrars)


---
# 2. Nuestra primera página

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

### Preparando una página de inicio con Atom y Markdown Preview Enhanced

### Cosas avanzadas

Si quieres, por ejemplo, poder saber [en qué enlaces de tu web hace más clic la gente](https://www.digitalocean.com/community/tutorials/how-to-build-a-modern-web-application-to-manage-customer-information-with-django-and-react-on-ubuntu-18-04), o crear una web más avanzada, tendrás que aprender lo básico de javascript.

---
# 3. Subiendo los contenidos

## Exportando y subiendo a la web con un programa de FTP

Si lo haces todo con la terminal, con SSH estarás a gusto.

### Windows

Usa [Cyberduck](https://cyberduck.io/). Por el amor de dios, **NO USES FILEZILLA**. Intentará instalarte el [maldito McAfee](https://www.youtube.com/watch?v=DiN3rq6kqKI) que te destrozará el ordenador con AdWare.

### Mac (y Linux)

[Rclone](https://rclone.org/) tiene buena pinta, aunque aun no lo he probado y es para la terminal. Puedes sincronizar cosas con tu Drive o Dropbox.

Oh, me acabo de dar cuenta. [Cyberduck](https://cyberduck.io/) también está para Mac.

### Linux

Os buscais la vida, ya sabreis como va la vaina. Si conoces un buen software de FTP, dimelo y lo añadiré aquí.

## Subiendo los archivos desde un repositorio de Git o GitHub

Esta es la opción más deseable. Aún no lo he probado pero está todo en este video:

[![](http://img.youtube.com/vi/V5e12MQRiU8/0.jpg)](http://www.youtube.com/watch?v=V5e12MQRiU8 "")

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
