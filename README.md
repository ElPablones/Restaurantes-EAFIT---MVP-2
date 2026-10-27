# \[Restaurantes EAFIT\]

> **Qué es este archivo.** Es la portada del proyecto. Lo lee cualquier persona que llegue a la carpeta o al repositorio (tu docente, un compañero, alguien que quiera reutilizar el trabajo) y debe poder entender qué es, dónde verlo y cómo se hizo sin preguntarle a nadie. Se redacta como un borrador desde el inicio y se completa en la Fase 6\.

> **Cómo llenarlo.**

> - Reemplaza todo lo que está entre \[corchetes\] y borra estos bloques de instrucciones (las líneas que empiezan con `>`).  
> - Escríbelo pensando en alguien que nunca vio el proyecto. Prueba con un compañero: si con solo leerlo puede abrir el sitio y entender qué es, está bien.  
> - Es para personas, no para la IA. La IA lee `CONTEXTO.md`; las personas leen este archivo.  
> - No incluyas datos personales de participantes, contraseñas ni llaves de acceso.  
> - Mantenlo actualizado: cuando cambie la URL, la analítica o algo del equipo, cámbialo aquí.

---

\[App para pedir en los restaurantes de la Universidad de EAFIT\]

**Sitio publicado:** \[https\://tugui142.github.io/eafit-pedidos-mvp-HTML/index.html\] **Repositorio:** \[https\://github.com/Tugui142/eafit-pedidos-mvp-HTML\] **Equipo:** \[Juan Pablo Gutiérrez Quintero — rol\], \[Verónica Mejia — rol\], \[Alejandra Fonseca — rol\] **Curso:** Experiencia de Usuario (CS0278) · \[2026-II\] · Universidad EAFIT **Docente:** \[Luis Alejandro Cardenas Franco\]

## Qué es

> Propósito, usuarios y la evidencia de la investigación que sustenta el sitio, en pocas líneas. No copies todo el informe: resume y enlaza.

\[[https\://drive.google.com/drive/folders/1vIvaelYmluDm5y9j\_QRFQvIUQoIvglPE?ths=true](https://drive.google.com/drive/folders/1vIvaelYmluDm5y9j_QRFQvIUQoIvglPE?ths=true)&nbsp;

Es una solución digital integral diseñada para mitigar la congestión y las largas filas en los restaurantes del campus de la Universidad EAFIT durante las horas de mayor afluencia. Mediante pedidos anticipados, digitalización de los procesos y un modelo colaborativo, el proyecto busca mejorar la experiencia gastronómica universitaria.

* **Propósito:** Devolver a la comunidad universitaria el control efectivo de su tiempo de descanso y optimizar simultáneamente la capacidad operativa de los restaurantes locales, previniendo el colapso logístico en la atención presencial.  
* **Ecosistema de Usuarios:**  
  * **Usuarios principales:** Estudiantes, profesores y empleados de EAFIT que buscan maximizar y organizar eficientemente sus espacios libres entre clases o jornadas laborales.  
  * **Restaurantes Aliados:** Administradores y personal operativo de los restaurantes institucionales y de cadena del campus (como Frisby o El Corral).  
  * **Emprendedores Estudiantiles:** Estudiantes con iniciativas y negocios gastronómicos propios que utilizan la plataforma como vitrina comercial y canal logístico (apoyándose en la red de repartidores) para visibilizar, gestionar su stock diario y expandir sus ventas de forma organizada dentro de la universidad.  
  * **Repartidores (Delivery P2P):** Estudiantes que utilizan su tiempo libre para realizar entregas internas dentro del campus (entre bloques, aulas o zonas comunes), generando un ecosistema de economía colaborativa segura.  
* **Evidencia y Validación de Investigación:**  
  * **Validación del problema:** Las entrevistas de campo confirmaron tiempos de espera críticos (30-40 minutos) en horas pico, validando la necesidad de un ecosistema logístico cerrado tipo "Rappi universitario" exclusivo para la comunidad EAFIT.  
  * **Evaluación de usabilidad:** Las pruebas de concepto con el MVP web (mediante Paseo Cognitivo y Escala Likert) arrojaron altos niveles de satisfacción, con puntajes de 4.5 a 5.0 sobre 5 en criterios de facilidad de uso y claridad de interfaz. Estas pruebas permitieron identificar e implementar mejoras tempranas en el flujo de permisos de geolocalización.  
  * **Co-diseño y escalabilidad:** Las sesiones de Prototipado Colaborativo permitieron resolver fricciones del modelo inicial, derivando en la incorporación de funciones avanzadas como la gestión continua del carrito ("Seguir comprando"), una línea de tiempo interactiva para la trazabilidad de los pedidos (status tracker) y la estandarización de puntos de entrega por nomenclatura de bloques y aulas.\]

## Cómo ver el sitio en tu computador

> Pasos concretos para abrirlo en local. Si es un sitio estático, normalmente basta con abrir `index.html` en el navegador.

1. Descarga o clona la carpeta del proyecto.  
2. \[Abre `index.html` en el navegador / usa la extensión o el comando que usen para un servidor local.\]

## Cómo se publica

> Para que cualquiera del equipo pueda volver a publicar sin ti.

- Servicio: \[GitHub Pages / Netlify / Cloudflare Pages / hosting contratado\]  
- Pasos: \[por ejemplo: hacer commit, subir a la rama `main`, el servicio publica automáticamente / subir los archivos con el administrador de archivos\]  
- Importante: subir siempre juntos el CSS y todas las páginas modificadas.  
- Administra la cuenta: \[nombre\]

## Analítica y privacidad

> Qué se mide, con qué herramienta y dónde se ven los datos. Menciona el aviso de consentimiento.

- Herramienta: \[Microsoft Clarity / Google Analytics 4 / otra\]  
- Eventos medidos: \[lista del plan de medición\]  
- Dónde ver los datos: \[nombre de la cuenta o panel; sin claves\]  
- Fecha de activación: \[AAAA-MM-DD\]  
- Aviso de privacidad y consentimiento: \[dónde aparece en el sitio\]

## Estructura de la carpeta

```
[nombre-del-proyecto]/
  CONTEXTO.md   contexto del proyecto para la IA
  BITACORA.md   decisiones y uso de IA
  README.md     este archivo
  index.html    página de inicio
  paginas/      resto de las páginas
  css/          estilos.css (hoja de estilos única)
  js/           scripts
  img/          imágenes
  docs/         insumos de la investigación (sin datos personales)
```

&nbsp;

## Uso de IA

> Declara con honestidad qué herramientas usaron y para qué. El detalle está en la bitácora.

- Herramientas: \[Gemini, Notebook LM\]  
- Para qué se usaron: \[esqueleto de páginas, CSS, análisis de entrevistas \]  
- Qué decidió el equipo sin la IA: \[arquitectura de información\]  
- Registro completo: ver `BITACORA.md`.

## Créditos y licencias

> Todo recurso de terceros va aquí: imágenes, fuentes tipográficas, íconos, librerías.

- Imágenes: \[origen y licencia\]  
- Tipografías: \[nombre y fuente\]  
- Otros recursos: \[lista\]
