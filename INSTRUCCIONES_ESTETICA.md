# Instrucciones esteticas / HTML recomendaciones Antic

## Direccion general

El documento funciona como una pieza web de recomendacion interna para Antic Teatre. La estetica parte de la identidad visual del Antic: alto contraste, amarillo acido, azul electrico, negro, blanco, tipografia pesada en italica y composicion ligeramente inclinada.

La maqueta debe sentirse directa, escenica y grafica, evitando una apariencia institucional o de dossier corporativo. La logica visual es mas cercana a cartel, hoja de sala, fanzine digital y documento de trabajo.

## Paleta

- Amarillo acido: `#fbff1f`
- Azul electrico: `#0600ff`
- Negro: `#050505`
- Blanco: `#ffffff`

El amarillo se usa como fondo general, acento de tarjetas y bloques de recomendacion. El azul organiza navegacion, titulos, bordes y jerarquia. El negro se reserva para texto principal, sombras, lineas duras y contraste.

## Tipografia

- Fuente base: `Helvetica, Arial, sans-serif`
- Titulos: mayusculas, peso `900`, cursiva, azul.
- Botones y etiquetas: mayusculas, peso `900`, cursiva.
- Cuerpo: Helvetica/Arial, peso normal o semibold, sin decoracion excesiva.

No usar tipografias externas para evitar errores de carga y caracteres raros. Todo debe funcionar offline/local y en Netlify/GitHub Pages.

## Composicion

- Documento de una sola pagina HTML con secciones verticales.
- Portada con logo, contexto, titulo y seis tarjetas de acceso.
- Cada propuesta tiene:
  - imagen grande arriba;
  - titulo y artista;
  - etiquetas de procedencia/tipo;
  - texto descriptivo;
  - bloque amarillo para recomendacion personal;
  - materiales encontrados;
  - contacto y enlaces;
  - navegacion inferior.

## Imagenes

Las imagenes salen de los propios dossiers o materiales de las piezas. Deben verse completas y no como decoracion abstracta. Se usa `object-fit: contain` para no recortar informacion importante.

En futuras versiones, si hay capturas de video mejores que las portadas de dossier, conviene sustituirlas por frames mas escenicos.

## Botones y tarjetas

Los botones mantienen una inclinacion tipo fanzine mediante `skew`. La inclinacion debe ser visible pero controlada, para que el texto siga siendo legible.

Estructura:

- Tarjetas de portada: borde azul, fondo blanco, hover amarillo.
- Botones de materiales: borde azul, texto azul, fondo blanco.
- Contactos: fondo amarillo, borde negro.
- Navegacion: botones pequenos azules, tres columnas.

## Navegacion

La navegacion inferior se organiza en tres columnas:

```text
Ines       Raquel      Andrea
KET        Alina       Patricio
Inicio     Anterior    Siguiente
```

La idea es que sea util y tambien grafica. No hace falta que todas las flechas sean estrictamente funcionales si el conjunto ayuda a orientarse visualmente.

## Tono editorial

Cada ficha separa tres capas:

- descripcion objetiva de la pieza;
- por que podria interesar a Antic;
- recomendacion personal de Adrian, todavia editable.

La recomendacion personal debe sonar cercana y situada, sin parecer una nota oficial de Antic.

## Reglas practicas

- Mantener todo en un solo `index.html` y una carpeta `assets`.
- Evitar dependencias externas.
- No usar scripts salvo que sea imprescindible.
- Comprobar siempre que:
  - cargan todas las imagenes;
  - los enlaces locales a PDF funcionan;
  - el HTML no se desborda horizontalmente en escritorio;
  - la version movil conserva lectura y navegacion.

## Publicacion

Para Netlify o GitHub Pages basta con subir la carpeta:

```text
CATALUNYA_HTML/
  index.html
  assets/
```

Si se publica online, revisar antes los contactos personales y enlaces privados de Drive.
