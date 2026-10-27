# Bitácora del proyecto: Restaurantes EAFIT

> **Qué es este archivo.** Es el diario del proyecto. Registra qué hicieron, qué le pidieron a la IA, qué les devolvió y qué decidió el equipo, con la evidencia que lo respalda. Sirve para tres cosas: defender el trabajo en la sustentación, mostrar qué decidieron ustedes y qué ejecutó la IA, y reunir material para la Entrega 4\.

> **Cómo llevarla.**

> - Agrega una entrada nueva **al final** después de cada cambio importante: una decisión de diseño, un cambio de estructura, un uso significativo de la IA, un hallazgo de una prueba. No hace falta anotar cada pequeño ajuste.  
> - **Nunca borres entradas viejas**, ni las equivocadas. Si algo estaba mal, escribe una entrada nueva que lo corrija y la relacione con la anterior.  
> - Cada entrada nombra a quien trabajó. Todos los integrantes deben aparecer.  
> - En "Evidencia" apunta al hallazgo de la investigación, a la prueba con usuarios o al resultado de una herramienta que respalda la decisión. Si no hay evidencia, escríbelo: "sin evidencia, decisión del equipo por \[motivo\]".  
> - Resume el prompt, no pegues conversaciones enteras. Si es largo, guarda el enlace al chat o el archivo en `docs/`.  
> - No incluyas datos personales de participantes ni credenciales.  
> - Borra estos bloques de instrucciones (las líneas que empiezan con `>`) y la entrada de ejemplo cuando empieces.

---
---

## Plantilla de entrada (copia y pega una nueva por cada cambio importante)

### \[AAAA-MM-DD\] · \[Nombre de quien trabajó\]

- **Objetivo del cambio:** \[qué se quería lograr\]  
- **Prompt clave:** \[texto resumido, o enlace al chat\]  
- **Qué produjo la IA:** \[resumen de lo que devolvió, incluidos errores o cosas que inventó\]  
- **Decisión del equipo:** \[aceptado / ajustado / descartado\] porque \[motivo\]  
- **Evidencia que lo sustenta:** \[hallazgo, prueba o resultado de herramienta\]  
- **Archivos modificados:** \[lista\]  
- **Commit:** \[mensaje del commit\]  
- **Verificación:** \[qué se comprobó y cómo: navegador, 375 px, consola, herramienta externa\]

---

# **Bitácora del proyecto: Restaurantes EAFIT**

### **2026-09-12 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Construir la arquitectura base del MVP (flujo móvil para estudiantes, vista de escritorio para restaurantes y conexión con Google Sheets mediante FastAPI y Render).  
* **Prompt clave:** "Generar las vistas HTML mobile-first para inicio de sesión, catálogo, detalle de producto, facturación, seguimiento, historial y ajustes, además de un dashboard de cocina y un backend en Python (main.py) que conecte el frontend con Google Sheets."  
* **Qué produjo la IA:** El código completo de las pantallas en escala de grises usando Tailwind CSS por CDN, manejo de carrito y mensajería por localStorage, y el script main.py con los endpoints /nuevo-pedido y /pedidos conectados a gspread.  
* **Decisión del equipo:** Aceptado. Se validó la estructura general y se desplegó el backend en Render y el frontend en GitHub Pages (eafit-pedidos-mvp-HTML).  
* **Evidencia que lo sustenta:** Investigación inicial de tiempos de espera en plazoletas del campus → Necesidad de separar la experiencia móvil ágil del estudiante de la pantalla operativa del restaurante.  
* **Archivos modificados:** index.html, catalogo.html, producto.html, pago.html, seguimiento.html, historial.html, ajustes.html, restaurantes.html, dashboard.html, main.py, requirements.txt.  
* **Commit:** Update index.html, Update main.py, Update requirements.txt (carga inicial del MVP).  
* **Verificación:** Prueba de extremo a extremo enviando un pedido desde pago.html y comprobando la escritura de la fila en la hoja de cálculo eafit-pedidos-mvp.

### **2026-09-15 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Estandarizar la identidad visual del prototipo aplicando la paleta de colores institucional de EAFIT y la tipografía oficial (Inter), pasando de un wireframe en grises a media fidelidad.  
* **Prompt clave:** "Dejemos el style.css hecho de una vez con las variables de color de EAFIT y dime qué cambio en todos los códigos que tengo (cuidando no perder la animación .fade-in del index.html)."  
* **Qué produjo la IA:** Un archivo style.css centralizado con las variables :root de EAFIT, las reglas .hide-scroll, los estilos de los interruptores (toggle) y la animación @keyframes fadeIn. Además, entregó un bloque \<head\> universal con la extensión del tema en tailwind.config.  
* **Decisión del equipo:** Aceptado. Se migraron los estilos en línea de cada archivo hacia style.css y se reemplazaron las clases grises por los colores institucionales (eafit-oscuro, eafit-claro, eafit-amarillo).  
* **Evidencia que lo sustenta:** Heurística de consistencia y estándares visuales → El usuario identifica la plataforma como un servicio propio del ecosistema universitario.  
* **Archivos modificados:** style.css, index.html, catalogo.html, producto.html, pago.html, seguimiento.html, historial.html, ajustes.html, restaurantes.html, dashboard.html.  
* **Commit:** Update style.css.  
* **Verificación:** Revisión visual en navegador de escritorio comprobando el cambio de colores, tipografía y funcionamiento de la transición inicial en el login.

### **2026-09-15 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Crear las páginas individuales para los 22 restaurantes del campus dentro de una subcarpeta dedicada para conectar los botones "Ver" de restaurantes.html.  
* **Prompt clave:** "Dame un HTML para cada uno de los 22 restaurantes para empezar a tener los links como son en restaurantes.html. Los quiero guardar dentro de una subcarpeta en GitHub."  
* **Qué produjo la IA:** Inicialmente la IA sugirió usar una sola plantilla dinámica con parámetros por URL (?nombre=). Al solicitarle mantener archivos físicos separados en una carpeta, entregó la plantilla HTML base adaptada con la ruta relativa ../style.css y la tabla de referencia para los 22 locales.  
* **Decisión del equipo:** Rechazada la propuesta de plantilla única por URL; se decidió crear la subcarpeta restaurantes/ con archivos HTML individuales (ej. bigos.html, chipstation.html). Sin evidencia de usuarios, decisión del equipo por control directo de la estructura en GitHub y facilidad para personalizar cada menú más adelante. Durante la creación se corrigió un error de ruta en GitHub eliminando el slash inicial (/restaurantes/... → restaurantes/...).  
* **Evidencia que lo sustenta:** Sin evidencia, decisión del equipo por organización modular del repositorio.  
* **Archivos modificados:** restaurantes/bigos.html, restaurantes/chipstation.html (y demás locales en restaurantes/), restaurantes.html.  
* **Commit:** Create bigos.html, Create chipstation.html, Update restaurantes.html.  
* **Verificación:** Navegación desde restaurantes.html hacia los archivos dentro de restaurantes/ verificando que carguen el ../style.css sin perder estilos.

### **2026-10-18 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Mejorar la visualización del mapa del campus (uMap) y hacer interactivo y realista el gráfico de "Demanda actual" en catalogo.html.  
* **Prompt clave:** "Ayúdame a mejorar el mapa para que sea más grande al abrir y más interactuable. Y mejoremos lo de demanda actual, que sea un gráfico interactivo y real."  
* **Qué produjo la IA:** Un modal ampliado (h-\[82vh\]) para el iframe de OpenStreetMap/uMap y un script de Chart.js con datos desde las 8am hasta las 6pm, colores dinámicos según congestión y *tooltips* personalizados ("Alta congestión", "Demanda moderada", "Flujo normal"). En la primera integración se duplicó una etiqueta \<script\> y faltó el CDN de Chart.js, dejando la pantalla en blanco; además se había recortado el arreglo menuDB.  
* **Decisión del equipo:** Ajustado. Se solicitó a la IA corregir las etiquetas \<script\> rotas, reincorporar el CDN de Chart.js y restaurar el filtro por categorías (Todos, Hamburguesas, Sushi, Pollo) junto con los platos del catálogo.  
* **Evidencia que lo sustenta:** Hallazgo del planteamiento del problema (los estudiantes necesitan prever qué tan llenas están las plazoletas en horas pico como las 12m y 1pm antes de decidir dónde pedir) y prueba de renderizado en navegador (catalogo.html en blanco antes de la corrección).  
* **Archivos modificados:** catalogo.html.  
* **Commit:** Update catalogo.html.  
* **Verificación:** Comprobado en navegador que el gráfico anima las barras al cargar, muestra los globos informativos al pasar el cursor/dedo y filtra los productos por categoría sin errores en consola.

### **2026-10-19 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Solucionar el fallo de renderizado visual en navegadores móviles (Safari y Chrome en iOS), donde la aplicación se veía sin estilos y con el menú lateral y el mapa desplegados en texto plano.  
* **Prompt clave:** "Mira cómo luce en el celular en Safari y en Google (capturas adjuntas). El style.css sí está en el repositorio, ¿cómo hago para que funcione?"  
* **Qué produjo la IA:** Diagnóstico de caché estática agresiva en navegadores móviles con GitHub Pages, sumado a un código de respaldo con estilos en el \<head\> e instrucciones para limpiar caché o usar parámetros de versión (?v=2.0).  
* **Decisión del equipo:** Se probó primero en pestaña de incógnito desde el celular sin alterar la arquitectura de archivos y se confirmó que el código ya funcionaba correctamente; finalmente se limpió la caché del navegador móvil.  
* **Evidencia que lo sustenta:** Pruebas de visualización en dispositivo móvil real (iPhone en Safari y Chrome a las 2:57 PM y 3:13 PM) comparadas contra la prueba en modo incógnito.  
* **Archivos modificados:** Ninguno (validación de despliegue en GitHub Pages).  
* **Commit:** N/A (verificación de entorno).  
* **Verificación:** Apertura de tugui142.github.io en móvil mostrando colores institucionales, menú lateral oculto por defecto (-translate-x-full) y modal del mapa cerrado hasta hacer clic.

### **2026-10-20 · Juan Pablo Gutiérrez**

* **Objetivo del cambio:** Rediseñar dashboard.html para pasar de un tablero Kanban estático de un solo local a una **línea de tiempo cronológica (tipo horario)** conectada en tiempo real a Google Sheets mediante Render, incluyendo los 22 restaurantes, un botón de campana (🔔) para alertas y botón de cierre de sesión.  
* **Prompt clave:** "Dame un dashboard mejorado donde se pueda elegir entre los 22 restaurantes, agrega un botón de campana en vez de decir 'Mensajes', un botón para volver al index, y que el dashboard sea una línea de tiempo tipo horario conectada al Sheet en tiempo real."  
* **Qué produjo la IA:** En una primera versión incluyó solo 7 restaurantes; tras pedirle la corrección, entregó el dashboard.html completo con los 22 locales en el \<select\>, el botón de notificación con insignia animada (🔔), el botón Salir hacia index.html, y la función fetchPedidosFromSheets() que consulta \[https\://eafit-pedidos-mvp-html.onrender.com/pedidos\](https\://eafit-pedidos-mvp-html.onrender.com/pedidos) y ordena las órdenes por hora de recogida (a.time.localeCompare(b.time)).  
* **Decisión del equipo:** Aceptado el rediseño a línea de tiempo y la lectura en tiempo real (GET /pedidos). Se decidió mantener el botón "Marcar Listo ✓" como simulación visual (alert) sin crear un endpoint PUT/PATCH adicional en el backend, dado que cumple el alcance necesario para las pruebas del MVP.  
* **Evidencia que lo sustenta:** Necesidad operativa del usuario "Restaurante/Cocina": en horas pico de almuerzo es más útil priorizar la preparación por hora exacta de recogida comprometida que por columnas sin orden temporal.  
* **Archivos modificados:** dashboard.html.  
* **Commit:** Update dashboard.html.  
* **Verificación:** Revisión en pantalla de escritorio verificando el selector de los 22 locales, la alerta visual en la campana al enviar un mensaje desde seguimiento.html, la carga de pedidos desde Render ordenados por hora y el retorno a index.html con el botón "Salir".

&nbsp;
