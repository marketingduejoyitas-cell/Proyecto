# Informe: estructura de categorías de duejoyitas.es

**Fecha de la revisión:** 6 de noviembre de 2026
**Método:** lectura de las páginas públicas de la tienda (menú y las 48 categorías). **No se ha modificado nada en la tienda.**
**Datos en bruto:** `categorias_actuales_duejoyitas_2026-11-06.csv` (categoría, URL, nº de productos, título y descripción SEO).

---

## 1. Resumen

- La tienda tiene **6 categorías principales en el menú, más Personalizada, Boda y Special Prices, y 39 subcategorías**, con unos 650 productos.
- El problema no es tener subcategorías, sino **mezclar tres criterios distintos** dentro de cada categoría:
  1. **Forma o tipo:** eternidad, sello, aros, largos… ✅ Esto sí debe ser subcategoría.
  2. **Piedra:** circonitas, piedras naturales, perlas. ⚠️ Solo cuando hay búsquedas y suficientes productos.
  3. **Acabado:** bañado en oro, chapado en oro, bañado en rodio. ❌ Esto debería ser un **filtro**, no una subcategoría.
- **No hay filtros activos** en las páginas de categoría: no se detecta la Búsqueda facetada. Por eso las subcategorías de acabado intentan hacer el trabajo de un filtro.
- Cada producto de anillos está en **3 o 4 subcategorías de media**. Así muchas páginas muestran casi los mismos productos, y eso confunde a la clienta y a Google.
- Lo bueno: **todas las categorías ya tienen título SEO, meta descripción y un texto de unas 250-300 palabras.** Esa base hay que conservarla.

**Respuesta a tu pregunta:** no te conviene quedarte solo con categorías. Lo mejor es **reducir a unas 30 subcategorías bien elegidas, activar filtros y añadir 2 secciones nuevas (Regalos y Novias)**. Así pasas de 48 a unas 38 categorías, pero mucho más claras.

---

## 2. Cómo está la tienda hoy

| Categoría | Productos | Subcategorías (nº de productos) |
|---|---|---|
| **Anillos** | 139 | Básicos (72), Eternidad (18), Solitarios (31), Sello (10), Anchos (22), Piedras naturales (59), Circonitas (90), Bañados en oro (45), Chapados en oro (6), Bañados en rodio (80) |
| **Colgantes** | 106 | Con piedras (63), Con perlas (9), Medallas (8), Gargantillas (43), Chokers (6), Pequeños (60), Cruz (5), Bañados en oro (20), Chapados en oro (12), Bañados en rodio (23), Collar (29) |
| **Pulseras** | 39 | Finas (27), Brazaletes (12), Con piedras (22), Con perlas (1), Bañadas en oro (16), Chapadas en oro (7), Bañadas en rodio (8) |
| **Pendientes** | 189 | Con piedras (98), Con perlas (16), Aros (28), Largos (72), Botón (27), Presión (45), Bañados en oro (28), Chapados en oro (18), Bañados en rodio (80) |
| **Oro** | 129 | Anillos de oro (122), Pendientes de oro (3), Colgantes de oro (4) |
| **Personalizada** | 6 | — |
| **Boda** | 38 | — |
| **Special Prices** | 45 | — |

## 3. Problemas detectados

1. **El acabado como subcategoría.** "Bañados en rodio" tiene 80 de los 139 anillos y 80 de los 189 pendientes. Casi nadie busca "anillo bañado en rodio", y la diferencia entre *bañado* y *chapado* en oro no la entiende la clienta.
2. **Subcategorías con muy pocos productos:** Pulseras de perlas (1), Pendientes de oro (3), Colgantes de oro (4), Colgante cruz (5), Chokers (6), Anillos chapados en oro (6), Pulseras chapadas en oro (7). Google las ve como páginas pobres y dan sensación de tienda vacía.
3. **"Collar" dentro de Colgantes es confuso.** Contiene sobre todo colgantes y medallas (Virgen del Carmen, Virgen Niña…), y 21 de sus 29 productos también están en Gargantillas.
4. **Las medallas están repartidas** entre Medallas, Collar y Colgantes pequeños.
5. **Productos sin subcategoría:**
   - Anillos: JOLIE, PAULINE e YVONNE.
   - 14 pendientes, varios de ellos **aros** que no están en "Pendientes aros": Aros DELOS Oro, LINE AROS, CIRCLE, DUOCIRCLE, TRICIRCLE, SPIRAL Grande y otros.
6. **URL repetida:** "Pendientes bañados en oro" (`127-pendientes-con-oro`) y "Pendientes chapados en oro" (`128-pendientes-con-oro`) comparten la misma URL de texto.
7. **El nombre y la URL no coinciden:** "Pendientes de presión" está en `126-pendientes-de-clic`, y "Colgantes pequeños" en `114-colgantes-mini`.
8. **"Special Prices" está en inglés** en una tienda en español.
9. **Faltan secciones** que tu plan de Black Friday y Navidad necesita como página de destino de los anuncios: Ideas de regalo, Anillos de compromiso y Novias e invitadas.

---

## 4. Estructura propuesta

Leyenda: **[mantener]** se queda como está · **[renombrar]** solo cambia el nombre · **[fusionar]** se junta con otra · **[nueva]** hay que crearla · **[filtro]** se elimina como categoría y pasa a ser un filtro.

### ANILLOS (`12-anillos-de-plata`) [mantener]
- Anillos de eternidad (`103`) [mantener]
- Anillos solitarios (`104`) [mantener]
- Anillos de sello (`105`) [mantener]
- Anillos anchos (`106`) [mantener]
- Anillos minimalistas (`102`) [renombrar "Básicos" → "Minimalistas", que es como lo busca la gente]
- Anillos con piedras naturales (`107`) [mantener]
- Anillos de circonitas (`108`) [mantener]
- **Anillos dorados** (`110`) [fusionar Bañados en oro y Chapados en oro (`111`)]
- ~~Anillos bañados en rodio (`112`)~~ [filtro]
- *Enlace en el menú:* Anillos de oro → lleva a ORO

### PENDIENTES (`14-pendientes-de-plata`) [mantener]
- Pendientes de aro (`41`) [mantener; añadir los aros que faltan]
- Pendientes largos (`124`) [mantener]
- Pendientes de botón (`125`) [mantener]
- Pendientes de presión (`126`) [mantener; corregir la URL o el nombre para que coincidan]
- Pendientes con piedras (`33`) [mantener]
- Pendientes de perlas (`31`) [mantener]
- **Pendientes dorados** (`127`) [fusionar Bañados y Chapados en oro (`128`); así se resuelve también la URL repetida]
- ~~Pendientes bañados en rodio (`129`)~~ [filtro]

### COLLARES Y COLGANTES (`3-colgantes-de-plata`) [renombrar: "collares" se busca mucho más]
- Colgantes con piedras (`28`) [mantener]
- Colgantes de perlas (`30`) [mantener]
- **Medallas y cruces** (`38`) [fusionar Medallas, Cruz (`29`) y las medallas que hoy están en Collar]
- **Gargantillas y chokers** (`32`) [fusionar Gargantillas y Chokers (`113`)]
- Colgantes pequeños (`114`) [mantener]
- **Colgantes dorados** (`117`) [fusionar Bañados y Chapados en oro (`118`)]
- ~~Collar (`34`)~~ [eliminar; sus productos ya están en otras subcategorías]
- ~~Colgantes bañados en rodio (`119`)~~ [filtro]

### PULSERAS (`13-pulseras-plata`) [mantener]
- Pulseras finas (`120`) [mantener]
- Brazaletes (`35`) [mantener; revisar que todos sean brazaletes, porque hay pulseras de cadena y de hilo]
- Pulseras con piedras (`46`) [mantener; meter aquí la única pulsera de perlas]
- **Pulseras doradas** (`121`) [fusionar Bañadas y Chapadas en oro (`122`)]
- ~~Pulseras de perlas (`37`)~~ [eliminar: tiene 1 producto]
- ~~Pulseras bañadas en rodio (`123`)~~ [filtro]

### ORO (`51-oro`) [mantener como línea propia y diferenciada, como dice el plan]
- Anillos de oro (`47`) [mantener]
- **Pendientes y colgantes de oro** (`130`) [fusionar Pendientes y Colgantes de oro (`131`), que tienen 3 y 4 productos; volver a separarlos cuando cada uno tenga 8 o más]

### NOVIAS E INVITADAS (`49-boda`) [renombrar]
- **Anillos de compromiso** [nueva: solitarios y anillos de eternidad, de plata y de oro con diamante]
- Joyas de novia [nueva: los 38 productos actuales de Boda]
- Joyas para invitadas [nueva, opcional]

### REGALOS [nueva, la del plan de Navidad]
- Regalos de menos de 50 € [nueva]
- Regalos de menos de 100 € [nueva]
- Packs de regalo [nueva]
- Joyas personalizadas (`17`) [mover aquí]
- Tarjeta regalo [nueva]

### OFERTAS (`66-special-price`) [renombrar "Special Prices" → "Ofertas"; reutilizar en Black Friday]

### COLECCIONES [nueva, opcional]
- Cordelia Art Déco, Azucena… Las colecciones con historia de tu plan, cuando estén montadas.

---

## 5. Filtros que hay que activar

Se activan con el módulo **Búsqueda facetada** (`ps_facetedsearch`), que viene incluido en PrestaShop. Para que funcionen, los productos tienen que tener rellenas las **Características** correspondientes.

| Filtro | Valores | Dónde |
|---|---|---|
| Acabado | Plata, Bañado en oro, Bañado en rodio, Oro rosa, Bicolor | Toda la plata |
| Piedra | Circonita, Perla, Piedra natural (esmeralda, zafiro, rubí…), Sin piedra | Todas |
| Color | Blanco, Verde, Azul, Rojo… | Todas |
| Precio | Rangos | Todas |
| Talla | Tallas de anillo | Anillos |
| Cierre | Presión, Botón, Aro, Gancho | Pendientes |

---

## 6. Cómo hacer el cambio sin perder posicionamiento

1. **No cambiar las URL de las categorías que se mantienen**, aunque cambie el nombre visible. Las URL actuales ya tienen historial en Google.
2. **Cada categoría que se elimine o fusione necesita una redirección 301** hacia la categoría que la sustituye. Por ejemplo, `111-anillos-chapados-en-oro` → `110-anillos-con-oro`. En PrestaShop 8 se configura en la propia categoría; en la 1.7 hace falta un módulo o `.htaccess`.
3. **Primero activar los filtros y rellenar las características**, y solo después quitar las subcategorías de acabado. Si se hace al revés, la clienta pierde la forma de encontrar esos productos.
4. **Aprovechar los textos SEO ya escritos** de las categorías fusionadas en la categoría que queda.
5. **Calendario recomendado:** por el Black Friday, ahora solo crear las secciones nuevas (Regalos, Anillos de compromiso y Ofertas) y corregir los aros sin categoría. Las fusiones y eliminaciones, en **enero**, con la tienda más tranquila.

## 7. Limitaciones de este informe

- Se ha hecho solo con las páginas públicas. No he visto el panel de PrestaShop, así que puede haber categorías ocultas que no salen en el menú.
- Las ideas sobre qué busca más la gente se basan en conocimiento general del sector. Antes de crear las categorías nuevas conviene confirmarlo en Search Console o en el Planificador de palabras clave de Google Ads.
