# Contexto del proyecto: Restaurantes EAFIT

> **Qué es este archivo.** Es la memoria del proyecto para la IA. Cada vez que abras una sesión nueva con la IA, pégalo o adjúntalo y pídele que resuma lo que entendió antes de hacer cualquier cosa. La IA no recuerda lo de ayer; este archivo sí.

> **Cómo llenarlo.**

> - Escríbelo entre todo el equipo. La IA puede ayudarte a ordenarlo, pero el contenido sale de ustedes y de su investigación.  
> - Reemplaza todo lo que está entre \[corchetes\].  
> - Borra estos bloques de instrucciones (las líneas que empiezan con `>`) cuando termines.  
> - Sé breve y concreto. Una IA lee mejor un texto corto y claro que uno largo.  
> - **No incluyas** nombres, correos, grabaciones ni datos identificables de los participantes de tu investigación. Usa códigos (P1, P2).  
> - Nunca escribas aquí contraseñas ni llaves de acceso.  
> - Actualiza solo la sección "Estado actual" al cerrar cada sesión. Las demás secciones cambian únicamente si cambia una decisión del equipo.

---

## 1\. Propósito

> Qué es el sitio y qué debe lograr, en 2 o 3 frases. Si no puedes explicarlo en tres frases, aún falta claridad (vuelve a la Fase 0).

\[Es una solución digital diseñada para mitigar la congestión y las largas filas en los restaurantes del campus de la Universidad EAFIT durante las horas de mayor afluencia o congestión. Busca devolver a la comunidad universitaria el control de su tiempo de descanso y optimizar la capacidad operativa de las cocinas mediante pedidos anticipados, y un modelo colaborativo para los estudiantes, ya sean emprendedores, o estudiantes con tiempo libre entre clases que deseen realizar pedidos a cambio de dinero.\]

## 2\. Usuarios y tareas principales

> Una línea por tipo de usuario: quién es y qué necesita hacer en el sitio. Salen de tu investigación, no de suposiciones.
  
- Usuarios principales (Estudiantes/Profesores/Empleados): necesitan realizar pedidos anticipados para recoger o recibir a domicilio, optimizando sus tiempos de descanso.  
- Restaurantes aliados: necesitan gestionar pedidos digitales de forma eficiente para evitar el colapso de la atención presencial.  
- Emprendedores estudiantes: necesitan una vitrina comercial y un canal logístico para gestionar su stock diario y expandir sus ventas en el campus.  
- Repartidores: necesitan aceptar y completar entregas internas dentro del campus para generar ingresos extra en sus tiempos de descanso.

&nbsp;

## 3\. Evidencia clave de la investigación

> Los hallazgos más importantes del ciclo Lean UX y la decisión que implican para el sitio. Esta tabla es la que le permite a la IA (y a tu docente) ver por qué el sitio es como es. Cada decisión de diseño debería poder rastrearse hasta una fila de aquí.

| Hallazgo (sin datos personales) | Estado (validada, refutada, inconclusa) | Decisión para el sitio |
| :---- | :---- | :---- |
| \[Frustración y colapso en horas pico: Los estudiantes tardan entre 30 y 40 minutos haciendo fila en restaurantes como Frisby o El Corral entre las 12:00 p. m. y 2:00 p. m., perdiendo su tiempo de descanso.\] | \[Validada\] | \[Implementar módulo de pedidos anticipados con selección de hora exacta de recogida y límite de cupos por franja horaria en cocina. \] |
| \[Privacidad del campus: Los usuarios conciben la solución como un "Rappi universitario" exclusivo y seguro. \] | \[Validada\] | \[Exigir autenticación con correo institucional @eafit.edu.co antes de ingresar al catálogo. \] |
| \[Fricción en el carrito del MVP web: El prototipo web redirige directamente al pago al elegir un producto, impidiendo añadir postres o acompañamientos. \] | \[Refutada (Flujo directo rechazado)\] | \[Rediseñar la pantalla de carrito para incluir la opción "Seguir comprando" antes de avanzar al checkout.\] |
| \[Desorientación de usuarios nuevos: Al ingresar por primera vez, los usuarios manifestaron confusión por no saber cómo activar su localización en el mapa.\] | \[Validada\] | \[Agregar pantalla emergente de onboarding inicial que solicite permisos de ubicación en tiempo real nada más ingresar.\] |
| \[Incertidumbre sobre el tiempo de entrega: Los estudiantes necesitan saber el estado exacto de su comida para planificar el retorno a clase. \] | \[Validada\] | \[Incorporar un Status Tracker (línea de tiempo interactiva) que muestre hitos: Pedido recibido ➔ En preparación ➔ En camino ➔ Entregado en bloque X. \] |
| \[Ubicación exacta en el campus: Para la entrega presencial o recolección, se requieren referencias específicas dentro de EAFIT. \] | \[Validada\] | \[Incluir campos obligatorios de destino (bloque, piso y salón o locker) en el resumen de compra.\] |
| \[Alta usabilidad y claridad visual: Calificaciones unánimes de 4.5 a 5.0 / 5 en la Escala Likert por interfaz limpia y búsqueda directa. \] | \[Validada\] | \[Mantener el diseño minimalista, enfocado en tarjetas de productos y filtros de restaurantes sin sobrecargar la pantalla. \] |

&nbsp;

## 4\. Alcance del MVP

> Lo que entra en esta entrega y lo que se deja para después. Así la IA no agrega funciones que no pedimos.

- **Entra:** \[lista de historias de usuario o funciones\]  
- **No entra por ahora:** \[lista\]

## 5\. Tecnología y restricciones

> Con qué se construye y dónde se publica. Si algo está prohibido o no se puede usar, dilo aquí.

- Tipo de sitio: \[sitio estático con HTML, CSS y JavaScript / otro\]  
- Frameworks o librerías permitidas: \[ninguna / cuáles\]  
- Dónde se publica: \[GitHub Pages / Netlify / Cloudflare Pages / hosting contratado\]  
- Formularios o datos de usuarios: \[servicio externo elegido / no aplica\]  
- Analítica: \[herramienta y eventos definidos en el plan de medición\]

## 6\. Estructura del sitio

> Una fila por página. Copia aquí tu mapa del sitio de la Fase 2\.

| Página | Archivo | Qué hace el usuario aquí (una frase) |
| :---- | :---- | :---- |
| Inicio | index.html | \[frase\] |
| \[página 2\] | \[paginas/archivo.html\] | \[frase\] |

&nbsp;

Carpetas del proyecto:

```
[nombre-del-proyecto]/
  CONTEXTO.md
  BITACORA.md
  README.md
  index.html
  paginas/
  css/        estilos.css
  js/
  img/
  docs/
```

&nbsp;

## 7\. Sistema visual

> Valores exactos, para que la IA no improvise. Todo el estilo vive en `css/estilos.css`.

- Color principal: \[\#------\] (acciones principales)  
- Color secundario: \[\#------\] (acciones secundarias)  
- Color de aviso o estado: \[\#------\] (por ejemplo, "Disponible próximamente")  
- Fondo: \[\#------\] · Texto: \[\#------\]  
- Tipografía de títulos: \[nombre\]  
- Tipografía de texto: \[nombre\]  
- Botones, tarjetas y etiquetas: \[descripción breve o referencia a la página modelo\]  
- Página modelo: \[archivo\]  
- Versión actual del CSS: \[por ejemplo, `estilos.css?v=20261013`\]

## 8\. Tono de voz y reglas de UX writing

> Salen de tu UX writing de la Entrega 2\.

- Tono: \[descripción en una frase\]  
- Frases cortas y verbos de acción en los botones ("Ver cronograma", no "Cronograma").  
- Cada imagen lleva texto alternativo que describa su función.  
- Los enlaces externos abren en pestaña nueva.  
- \[Otras reglas del equipo\]

## 9\. Reglas para la IA

> No las borres: son lo que convierte a la IA en copiloto. Puedes agregar las tuyas.

1. Usa los textos exactos que se te entregan. No inventes títulos, datos, cifras ni nombres.  
2. Si falta información, pregúntame antes de escribir.  
3. Un cambio por petición. Antes de escribir código, muéstrame un plan con los archivos que vas a tocar y los supuestos que haces. Espera mi aprobación.  
4. No uses estilos dentro de las páginas ni colores fuera de las variables del CSS.  
5. Marca lo pendiente como "Disponible próximamente".  
6. Dime qué archivos y líneas cambiaste.  
7. No toques lo que está en la sección "No tocar".  
8. Si no puedes verificar algo (por ejemplo, que los enlaces funcionen), dímelo; no afirmes que lo revisaste.  
9. \[Regla propia del equipo\]

## 10\. No tocar

> Archivos, secciones o decisiones que la IA no debe modificar.

- \[por ejemplo: la sección "Exploración autónoma" de la página 3\]  
- \[por ejemplo: los colores definidos en la sección 7\]

## 11\. Estado actual

> Esta es la única sección que se actualiza en cada sesión. Pide a la IA que te proponga la actualización al cerrar, y revísala antes de guardarla.

- **Terminado:** \[lista\]  
- **En curso:** \[lista\]  
- **Siguiente paso:** \[lista\]  
- **Pendiente de decisión del equipo:** \[lista\]  
- **Última actualización:** \[fecha\] por \[nombre\]
