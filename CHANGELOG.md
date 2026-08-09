# CHANGELOG — Reinos Matemáticos 2026

Historial completo de cambios del proyecto, de más reciente a más antiguo.
Ver el estado actual en [`README.md`](README.md) · Pendientes en [`ROADMAP.md`](ROADMAP.md).

---

## 2026-08-09

### S7 — Fichas públicas simplificadas y resoluciones corregidas (`0e91f94`)

- A07–A11_Publica.html: cada ficha muestra solo título, imagen ilustrada (HojaAlumno) con botones descargar/imprimir, y cita de fuente — sin contenido duplicado en texto.
- Resoluciones A07, A08, A10, A11 reconstruidas con las respuestas verificadas de los ítems Plan B públicos (las versiones anteriores resolvían ejercicios del libro con copyright).

### S7 — Fichas públicas completas, imágenes ilustradas y limpieza de fuentes (`183376e`, `0ce8d76`)

- A07/A08/A09_Publica.html actualizados (panel "Hoja ilustrada" al final); A10/A11_Publica.html trackeados por primera vez.
- Imágenes A07–A11_HojaAlumno_Imprimir.png desplegadas en cada carpeta de misión.
- Fuentes originales eliminadas del repo y archivadas en `Secuencia 7\Actividades`: A07_pag101_Porras.pdf, A08_pag17-19_vitabar.pdf, A09_pag102_Deberes.pdf, A09b_pag103_Deberes.png, A10_pag20-23_multiplicacion.pdf, A11_Cuadrado_Binomio.pdf.
- index.html de misiones 01–04 y 06 actualizados: cargan la ficha por iframe en vez del PDF original.
- mision-07/A12_Publica.html eliminado del working tree (A-12 dado de baja definitivamente).

### S7 — Limpieza de A-12, lecciones rediseñadas y huérfanos (`87273b5`, `3877121`)

- leccion-2.html: reemplazada con versión rediseñada (mismo tratamiento visual que L4/L5); ya no usa pag104_Porras_Leccion.png.
- leccion-4.html y leccion-5.html: reemplazadas con versiones del staging público.
- leccion-5.html: href del botón "← Lección 4" corregido (apuntaba a nombre de archivo de staging, no al del Reino).
- A-12 (Crucigrama) dado de baja: mision-07/ eliminada, A12_Crucigrama_Resolucion.html eliminada, Misión V removida del modal, contador 5→4 misiones, descripción actualizada.
- pag104_Porras_Leccion.png y pag107_Producto_Notable_Leccion.pdf eliminados del repo (ya sin referencias).

---

## 2026-08-05

### S8 cierre, biblioteca y misiones: segunda tanda (`TBD`)

- Creada `s8-ecuaciones/cierre/` con `index.html` (patrón S7: MC_HABILITADO=false, RESOLUCION_HABILITADA=false), `MC-S8_ficha.html` y `MC-S8_resolucion.html`.
- Biblioteca S8: agregada Lección 1 — Introducción a las ecuaciones; lecciones renumeradas (anterior L1→L2, anterior L2→L3). Hub actualizado con los tres títulos.
- `E11_ficha.html` corregida: eliminado el cuadro "trampa" que revelaba la ecuación antes del planteo del estudiante en el ítem 2.
- Mapa S8 (`index.html`): Biblioteca desbloqueada; E-09 eliminado del menú de misiones (pasa a Biblioteca); E-10 renombrado a Misión X; VIII=Bingo (E-07), IX=Baraja (E-06); contador actualizado a 10 misiones.

### S8 Biblioteca: publicadas L1 y L2 + E02 resolución actualizada (`1b24d3f`)

- Creada `s8-ecuaciones/biblioteca/` con hub `index.html` (patrón S7 — Cinzel, fondo pergamino).
- L1 — Lenguaje y equivalencia de ecuaciones: vocabulario, miembros, incógnitas, grado, los tres casos.
- L2 — El método de Polya: cuatro fases ilustradas con ejemplo del taxi de E02.
- `E02_resolucion.html` reemplazada por versión corregida (ruta al PDF de ficha ajustada a `../misiones/mision-02/`).
- Pendiente: cierre S8 (MC-S8) y desbloqueo de Biblioteca en el mapa del subreino.

---

## 2026-08-04

### S7 Biblioteca: Lección 5 — Cuadrado de un binomio versión gráfica (`36c5a8d`)

- Creada `s7-polinomios/biblioteca/leccion-5.html`: demostración visual por áreas del (a+b)².
- Hub `biblioteca/index.html` actualizado con tarjeta de Lección 5.
- `leccion-4.html` actualizada con botón "Siguiente → Lección 5".

### S8 menú: reubicar Freudenthal (E-08) a posición III (`e2d4131`)

- E-08 (Freudenthal) pasa de Misión IX a Misión III, inmediatamente después de E-02.
- Misiones III–IX renumeradas en consecuencia; hrefs a carpetas sin cambios.

### S7 cierre: deshabilitar MC-S7 (`e2d4131`)

- `MC_HABILITADO` → `false`. `RESOLUCION_HABILITADA` ya estaba en `false`.

### S6 cierre: correcciones MC-S6 (`9069fe1`)

- `mc_s6_resolucion_explicada.html`: eliminado inciso d (verificación x=4) de tarjeta 4.
- `mc_s6_actividades.html`: tarjeta 3 abierta — sin preasignar la letra a "bolas azules".
- `cierre/index.html`: botón descarga `MC_S6_v3_final.pdf` agregado al MC; botón PDF eliminado de la resolución.
- `MC_S6_v3_final.pdf` publicado; `mc_s6_resolucion_explicada.pdf` eliminado del repo.

### S7: mision-05 eliminada y Ochoviet reservado en S8 (`991b640`, `1ecd78c`)

- Carpeta `mision-05` (refuerzo mult huérfano) eliminada de S7.
- `areas_rectangulo_Ochoviet.pdf` (Ochoviet-Vitabar, actividad áreas con dos letras) guardado en `s8-ecuaciones/` sin código asignado.

### S7 cierre: bloquear resolución (`556774c`)

- `RESOLUCION_HABILITADA` → `false` en cierre S7 (MC sigue accesible mientras se corrige en clase).

---

## 2026-07-31

### S7 — Renumeración de actividades e integración del MC-S7 (`dd09b57`)

- Actividades renumeradas: el refuerzo de suma/resta (A-09) y el refuerzo de multiplicación (A-11 antiguo) quedan como materiales de deberes sin misión digital propia.
- Secuencia digital de S7 queda: A-07, A-08, A-10, A-11 (antes A-12 binomio), A-12 (antes A-13 crucigrama). Total: 5 misiones.
- Renombrados PDFs, páginas de misión y archivos de resolución para reflejar los nuevos códigos.
- Modal de misiones actualizado a "5 misiones disponibles".
- Mini control MC-S7 integrado en `s7-polinomios/cierre/`: `MC_HABILITADO=true`, `RESOLUCION_HABILITADA=true`.
- Desafío Final S7 desbloqueado en el mapa del subreino con enlace a `cierre/index.html`.
- Resoluciones desbloqueadas: A-08, A-10, A-11 (nueva), A-12 (nueva). A-07 ya estaba activa.
- Archivos `MC_S7_Polinomios.pdf` y `MC_S7_Resolucion_Explicada.html` movidos desde la raíz a `cierre/` con nombres en minúsculas.

### S7 — Correcciones editoriales y visuales (`8335b90`)

Cinco puntos corregidos:
1. Superposición de tarjetas en el mapa: se separaron territorios que quedaban encima.
2. Posición del Desafío Final: reubicado para no solaparse con el sello.
3. Texto de S2 en el mapa de Álgebra y Funciones ajustado.
4. Referencias a número de página eliminadas de los títulos de misiones.
5. Revisión general de coherencia de íconos y descripciones.

### S7 — Biblioteca restructurada (`25e55a3`, `02274dd`)

- Biblioteca reorganizada en 4 lecciones individuales con un hub de navegación en `biblioteca/index.html`.
- Lección 1: Suma y resta de polinomios en columna.
- Lección 2: Multiplicación — propiedad distributiva (imagen Porras).
- Lección 3: Multiplicación de polinomios en columna.
- Lección 4: Cuadrado de un binomio — producto notable (PDF Porras).
- Corregido texto del modal ("dos lecciones" → descripción real) y navegación interna.

---

## 2026-07-30

### S8 — El Equilibrio Oculto (Ecuaciones) (`baa22c3`)

- Creado subreino `algebra-funciones/s8-ecuaciones/` completo con 11 misiones.
- Misiones E01–E11 con PDFs, PNGs y fichas HTML interactivas.
- Versiones docente de E06 (Baraja) y E07 (Bingo) ocultas del sitio estudiantil.
- Resoluciones habilitadas para E02, E04, E05, E11.
- Biblioteca y cierre bloqueados — a crear en etapa posterior.

### S7 — Resoluciones y correcciones (`8e93685`, `2864366`, `83c8988`)

- Agregada resolución A-13 (crucigrama).
- Reemplazadas resoluciones A-08 y A-10 con versiones corregidas.
- Agregada resolución A-12 (binomio).
- Bloqueadas temporalmente resoluciones A-08 y A-10 mientras se corregían.
- Agregada página 103 a la misión mision-03 (refuerzo suma/resta).
- Limpieza de archivos sueltos en la raíz del repositorio.

### S7 — El Mundo de los Polinomios (`bb2b217`)

- Creado subreino `algebra-funciones/s7-polinomios/` con 7 misiones (A-07 a A-13 en ese momento).
- Reorganizada estructura de S8 en su propia carpeta.

---

## 2026-07-29

### S6 — Resoluciones y reestructura completa (`20e4f3a`, varios)

- Agregadas resoluciones HTML para A-01/A-02, A-04, A-05.
- Restructuración del reino en niveles: mapa de reino + páginas de subreino independientes.
- Subreinos marcados visualmente en el mapa del reino con territorios propios.
- Corregidas posiciones de territorios para evitar superposición con el título.
- Navegación de misiones corregida (enlaces relativos desde nivel `misiones/mision-XX/`).
- Completado Desafío Final S6 con sistema de dos toggles independientes.
- Lección 4 de la biblioteca — definiciones de monomios y polinomios con PDF.

---

## 2026-07-21

### Álgebra y Funciones — Misiones II–VI, Biblioteca y Cierre (`23fd295`)

- Misiones A-02 a A-06 publicadas (PDFs con visor embed + descarga).
- Mision A-03 marcada como Deberes.
- Biblioteca con 3 lecciones (variables, lenguaje algebraico, términos semejantes).
- Cierre S6 con `cierre/index.html` (ambos toggles en `false`).

---

## 2026-07-12

### Proporciones — Bitácora de cierre (`bef3900`, `ce4dbee`)

- Creada `Bitacora_Cierre_Proporcionalidad.html` con reflexión narrativa de cierre del reino.
- Corrección de tildes y eñes en el archivo.

---

## 2026-07-09

### Álgebra y Funciones — Reino inicial (`fe17c10`, `60c70e0`)

- Creada carpeta `algebra-funciones/` con:
  - Prólogo: "El misterio del número sin nombre".
  - Misión I (A-01): Las letras que ya conocíamos (PNG interactivo).
  - Portal actualizado con tarjeta del nuevo reino.
- README actualizado con descripción del nuevo reino.

---

## 2026-07-08

### Proporciones — Desafío habilitado, documentación (`441f7bc`, `ad5eef5`, `eb1a34a`)

- Desafío Final de Proporciones desbloqueado en el mapa del reino.
- README y ROADMAP actualizados.
- Applet v4 reservado en ROADMAP para el futuro reino de Funciones Lineales.

---

## 2026-06-14

### Applet Fábrica de Pintura v4 (`2bb0c6f`, `c85c703`)

- Nueva versión del applet con modo puntos, botón "Ver recta", botón "Reiniciar".
- Sin evaluación automática del valor de k — permite exploración abierta.
- Eliminado texto que revelaba conclusiones antes de que el estudiante explorara.

---

## 2026-06-06

### Reorg general y Las Tierras sin Mapa completo (`547c62c` y varios)

- `proporciones/` movida a su propia subcarpeta (reorganización raíz).
- Las Tierras sin Mapa publicadas: `index.html`, `intro.html`, actividades C34–C46, Simulador Panini.
- Corrección de actividad C43 y activación del simulador.
- Compresión de PDFs pesados para mejorar tiempo de carga.
- README reescrito con el estado del proyecto en ese momento.

---

## 2026-06-05

### Las Tierras sin Mapa — intro animada (`bcc3d6b`)

- Creada `tierras-sin-mapa/intro.html` con animación de entrada y citas cinematográficas.

---

## 2026-06-01

### Proporciones — Bitácora del explorador (`4a874f0`)

- Actualizada bitácora del explorador con material de cierre del reino.

---

## 2026-05-31

### Proporciones — Correcciones varias (`f0724a3`, `d4705a5`, `52b919a`, `c71fe7d`, `40ba21e`)

- Correcciones de incrustación de videos en biblioteca (Error 153 CREA con wmode=opaque — eliminado).
- Reemplazadas URLs de imágenes de Ceibal/Schoology por imágenes alojadas en el repo.
- Íconos temáticos agregados en la biblioteca.
- Corrección de rutas relativas de PDFs.
- Actualización de materiales de S4.

---

## 2026-05-30

### Proporciones — Fundación del reino (`0a47838` y varios)

- Portal `index.html` rediseñado: fondo claro, arquitectura modular de tarjetas por reino.
- Biblioteca con videos YouTube sin `wmode` y fondo legible.
- Imágenes movidas a carpeta local del proyecto.
- Prólogo del reino creado.
- Applets Ciudad de las Proporciones y Fábrica de Pintura integrados.

---

## 2026-05-29

### Reino Matemático inicial (`aeddab5`)

- Primera versión del sitio con estructura base.

---

## 2026-05-28

### Commit inicial (`14e8d94`, `2642417`, `c0e757a`, `c097058`)

- Repositorio creado.
- Ciudad de las Proporciones (applet interactivo).
- Fábrica de Pintura (primera versión del applet).
- README inicial.
