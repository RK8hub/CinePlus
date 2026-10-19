# CinePlus+ Dashboard

Un panel con estética de dashboard que muestra los beneficios de la tarjeta **CinePlus+ Premium de Cinemark Nicaragua** de forma más clara e intuitiva que la página oficial.

Es un proyecto *vibecodeado*: un scraping de la web de beneficios de Cinemark, hecho con ayuda de IA, que lee los datos públicos de la página oficial y los reorganiza en tarjetas filtrables.

**Página oficial:** https://www.cinemarkca.com/nicaragua/cinetotal

## Aviso importante

- Este proyecto **no es una fuente oficial** ni tiene relación con Cinemark.
- **No nos hacemos responsables de inconsistencias**, errores u omisiones en la información mostrada.
- Los beneficios, condiciones y vigencias pueden cambiar sin previo aviso.
- **Siempre verifica los beneficios en la [página original](https://www.cinemarkca.com/nicaragua/cinetotal)** antes de tomar una decisión o de ir al cine.
- Cinemark y CinePlus+ son marcas de sus respectivos dueños.

## Qué hace

- Muestra los beneficios de taquilla y dulcería en tarjetas, con sus condiciones desplegables.
- Permite filtrar por Taquilla, Dulcería y Cumpleaños.
- Resume lo esencial: precio, vigencia de la tarjeta, cashback y días restantes de las promociones.
- Avisa cuando la página oficial muestra datos que parecen contradecirse, como dos topes de cashback distintos.
- Se actualiza solo: consulta los datos de la página oficial cada vez que se abre.
- Si no puede conectarse, muestra los últimos datos guardados en tu navegador, con un aviso.

## Cómo funciona

Es un único archivo HTML, sin dependencias ni proceso de compilación. Al abrirse, consulta el Content API público que usa la propia página de Cinemark y procesa la respuesta en el navegador.

## Limitaciones

- Depende de que Cinemark mantenga su API accesible desde otros dominios (CORS). Si la bloquea, el panel mostrará un error o los últimos datos guardados.
- Si Cinemark cambia la estructura de sus datos, el panel puede mostrar información incompleta o incorrecta.
- Los textos «Antes de usarla» y «Reglas generales» son fijos y no se actualizan solos.
