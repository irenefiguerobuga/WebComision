
# Web Comisión de Festas San Benito da Rocha de Atios

Página web desarrollada para la Comisión de Festas San Benito da Rocha de Atios, una asociación local de O Porriño (Pontevedra).

El objetivo del proyecto es ofrecer un espacio donde consultar información sobre las fiestas, conocer las novedades de la comisión y permitir que los vecinos compartan sus fotografías y comentarios.

La web está desarrollada en gallego, adaptada a dispositivos móviles y actualmente se encuentra en funcionamiento.

## Web publicada

🌐 [Visitar la página web](https://sanbenitorochaatios.github.io/web/)

La web oficial está alojada en el GitHub de la comisión. Este repositorio contiene una copia del proyecto para mostrar su desarrollo y las tecnologías utilizadas.

## Funcionalidades

- Información sobre la comisión y la Tasca da Rocha.
- Consulta de horarios y ubicación mediante Google Maps.
- Apartado de próximos eventos y celebraciones.
- Galería fotográfica.
- Integración de publicaciones y Reels de Instagram.
- Enlaces a las redes sociales.
- Formulario para que los visitantes envíen fotografías y comentarios.
- Sistema de revisión y aprobación de las aportaciones antes de publicarlas.
- Protección del formulario mediante Cloudflare Turnstile.
- Información sobre privacidad y protección de datos.
- Diseño adaptable a ordenadores y móviles.

## Tecnologías utilizadas

| Tecnología | Uso |
|------------|-----|
| HTML5 | Estructura de la página |
| CSS3 | Diseño y adaptación a dispositivos móviles |
| JavaScript | Funcionalidades e interactividad |
| Supabase | Base de datos y almacenamiento de fotografías |
| PostgreSQL | Gestión de los comentarios y aportaciones |
| Supabase Edge Functions | Comunicación entre el formulario y la base de datos |
| Cloudflare Turnstile | Protección contra envíos automatizados |
| GitHub Pages | Publicación de la web oficial |

## Sistema de fotografías y comentarios

Una de las partes principales del proyecto es la sección **"Os vosos recordos"**, que permite a los visitantes compartir sus fotografías y comentarios.

El funcionamiento es el siguiente:

1. El visitante rellena el formulario y adjunta una fotografía o escribe un comentario.
2. Consulta la información de privacidad y acepta las condiciones de publicación.
3. Cloudflare Turnstile realiza una comprobación de seguridad.
4. La información se envía a Supabase.
5. Las aportaciones se guardan en la base de datos con estado pendiente.
6. La comisión revisa las fotografías y comentarios y decide si los publica.
7. Una vez aprobados, aparecen en la web.

Esto permite gestionar las aportaciones desde Supabase sin tener que modificar manualmente el código de la página.

## Estructura del proyecto

- `index.html`: página principal.
- `styles.css`: estilos generales.
- `script.js`: funcionalidades de la web.
- `config.js`: configuración de eventos y novedades.
- `recordos.css`: estilos de la sección de recuerdos.
- `recordos.js`: formulario y visualización de fotografías y comentarios.
- `recordos-config.js`: configuración pública de la conexión con Supabase y Cloudflare.
- `privacidade.html`: información de privacidad y protección de datos.
- `assets/`: imágenes y recursos de la web.

## Sobre el desarrollo

Este proyecto se ha realizado para una asociación real, con el objetivo de facilitar la comunicación con los vecinos y dar a conocer sus actividades.

Durante su desarrollo he trabajado con HTML, CSS y JavaScript, además de integrar una base de datos PostgreSQL mediante Supabase, configurar el almacenamiento de fotografías y conectar distintos servicios externos.

También he realizado adaptaciones para dispositivos móviles, pruebas de funcionamiento y actualizaciones de la web.

Es un proyecto que continúa en uso y que se va actualizando con nuevos eventos, fotografías y funcionalidades.

## Redes sociales

- [Instagram](https://www.instagram.com/san_benito_da_rocha_atios/)
- [Facebook](https://www.facebook.com/profile.php?id=61595234168492)
