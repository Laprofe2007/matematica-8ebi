# ROADMAP — Reinos Matemáticos 2026

Tareas pendientes, decisiones abiertas y trabajo futuro para el proyecto.
Ver el estado actual completo en [`README.md`](README.md).
Ver el historial de cambios en [`CHANGELOG.md`](CHANGELOG.md).

---

## Prioridad alta (próximos pasos inmediatos)

### S7 — El Mundo de los Polinomios

S7 completamente armada pedagógicamente. Fichas públicas, imágenes ilustradas, resoluciones y biblioteca (5 lecciones) publicadas.

- [x] **Fichas A07–A11 simplificadas** — solo imagen + botones, sin contenido duplicado. ✓
- [x] **Resoluciones A07/A08/A10/A11 corregidas** — respuestas de los ítems Plan B públicos. ✓
- [x] **Biblioteca S7** — 5 lecciones en `s7-polinomios/biblioteca/`. ✓
- [x] **A-12 dado de baja** — mision-07 eliminada del repo; 4 misiones activas. ✓
- [ ] **Habilitar MC-S7** cuando corresponda: `cierre/index.html`, `MC_HABILITADO = false` → `true`.
- [ ] **Habilitar resolución MC-S7** en momento posterior: `RESOLUCION_HABILITADA = false` → `true`.
- [ ] **Resolución A-09**: sin archivo (es tarea domiciliaria, sin clave de respuesta — mantener así salvo decisión expresa).

### S8 — El Equilibrio Oculto (Ecuaciones)

S8 completamente armada pedagógicamente. Biblioteca y cierre publicados; pendiente habilitar en clase.

- [x] **Biblioteca S8** — 5 lecciones + hub en `s8-ecuaciones/biblioteca/`. ✓
- [x] **Biblioteca desbloqueada en el mapa** — territorio activo, enlace a `biblioteca/index.html`. ✓
- [x] **Cierre S8 publicado** — `s8-ecuaciones/cierre/` con `index.html`, ficha y resolución. ✓
- [ ] **Habilitar MC-S8** cuando corresponda: `cierre/index.html`, `MC_HABILITADO = false` → `true`.
- [ ] **Habilitar resolución MC-S8** en momento posterior: `RESOLUCION_HABILITADA = false` → `true`.
- [ ] **Habilitar Desafío Final S8 en el mapa** — `s8-ecuaciones/index.html`, territorio `desafio`: `bloqueado: false`, `enlace: "cierre/index.html"`.
- [x] **Resoluciones E01–E05, E08, E10, E11** publicadas en `resoluciones/`. ✓
- [x] **E06/E07 retiradas** del reino por decisión docente (calendario). Carpetas mision-07/08 eliminadas. ✓

### S6 — Código de Letras

- [x] **MC-S6 aplicado en clase** (~clase 42) y corregido. ✓
- [x] **MC-S6 y resolución habilitados**: ambos toggles `true`. ✓
- [ ] **Resolución A-06**: habilitarla cuando esté lista (actualmente sin archivo en resoluciones/).
- [ ] **Resolución A-03**: habilitarla cuando esté lista (actualmente sin archivo).

### Las Tierras sin Mapa (S5)

- [ ] **Habilitar Desafío Final** si se utiliza mini control de Probabilidad/Estadística.

---

## Prioridad media (a futuro)

### Nuevas secuencias en Álgebra y Funciones

- [ ] **S9 — Funciones Lineales**: próximo subreino a crear. El Applet v4 (`proporciones/Fabrica_Pintura_Applet_v4.html`) está reservado para este subreino — es la actividad interactiva de recta y = kx. Crear `algebra-funciones/s9-funciones-lineales/` siguiendo el patrón de S7/S8.
- [ ] **S10 y siguientes** (si corresponde al año): mismo patrón de subreino autocontenido.

### Mejoras generales

- [ ] **Activar territorio S9 en el mapa del reino** (`algebra-funciones/index.html`) cuando se cree el subreino.
- [ ] **Resolución A-01 independiente** para S6: actualmente A-01 y A-02 comparten un solo HTML. Si se requiere separación, crear `A-01_Resolucion_Explicada.html`.
- [ ] **Bitácora de Álgebra y Funciones**: carpeta `bitacora/` referenciada en el ROADMAP anterior pero sin contenido. Crear cuando se cuente con el PDF.

---

## Decisiones abiertas

| Tema | Opciones | Estado |
|---|---|---|
| Applet v4 Fábrica de Pintura | Publicar en S9 / mantener local | Pendiente — NO publicar hasta decidir |
| Simulador Panini 2027 | Actualizar temporada o mantener 2026 | Para el año siguiente |
| Cierre Las Tierras sin Mapa | ¿Crear cierre interactivo? | Sin decidir |
| Material docente E06/E07 | Actividades retiradas del reino (decisión 2026-09-17) | Cerrado |

---

## Mejoras S8 — diferidas para después del curso 2026

**Estado: anotado, no ejecutar durante el curso 2026.** Acordado el 6/10/2026.

Los códigos de las fichas se dejan como están. El orden de las misiones del Reino es el de origen de la secuencia y se mantiene para este curso. El número de carpeta de misión no sigue al código de la ficha: las carpetas se numeraron por orden de creación. No se renumera nada; el número de misión se maneja como se pueda para no romper el sitio.

### Secuencia lógica de referencia

Problema que da lugar a la aparición de la ecuación → método → prácticas del método → problema que da lugar a la aparición de la segunda serie → método nuevo → práctica → problemas de contextualización, donde el estudiante arma y elige el método → evaluación.

El criterio que organiza todo esto es que no haya superposición en la introducción de dos métodos. En S8 la cantidad de problemas de práctica quedó bien calibrada. El desvío respecto de esta secuencia se debió a que la clase de visita de didáctica se preparó sobre la marcha, en el medio de la unidad, y al tiempo efectivamente disponible.

### Ajustes a realizar cuando termine el curso

1. **Separar E03 Práctica graduada en tres fichas independientes.** La Parte 1 usa inversión y debe ir después del método de inversión. Las Partes 2 y 3 usan los dos métodos y deben ir después de introducir la transposición.

2. **Mover E12 Las estalagmitas de la cueva antes de las Partes 2 y 3 de E03.** E12 es el problema que introduce la necesidad del método nuevo, así que su lugar lógico es antes de la práctica que lo aplica. Implica además cambiar el código dentro de la propia ficha ilustrada, no solo en el sitio.

3. **Revisar la ubicación de E04 y E05.** Hipótesis a analizar: E04 Jo y la consola de videojuegos funcionaría mejor a continuación de Pijama Death (E01), como alternativa o como refuerzo de esa ficha, en lugar de quedar como práctica de contextualización al final. Hay que verificar que el cambio no genere superposición en la introducción de métodos.

> Estos tres ajustes son solo del Reino. No afectan al Fichero de Actividades ni a la Secuencia didáctica de 2026, que quedan como registro de lo efectivamente implementado.

---

## Archivos que nunca deben subirse a git

- `proporciones/Fabrica_Pintura_Applet_v4.html` — reservado para S9
- `proporciones/Actividades/hoja docente Correccion a_S3_S4_v4.pdf` — uso interno docente
- `proporciones/Actividades/S4_Act5_ViajeEgresados_v2.pdf` — versión en revisión
- E05 source PDF — no incluir en el sitio
- E01 DOCX — no subir ni enlazar
- E02 resolución docente PDF — uso interno

---

## Decisiones de diseño ya tomadas (no reabrir)

- Fuentes: Cinzel + Libre Baskerville para mapas y portal; Nunito para misiones y resoluciones.
- Fondo: CLARO (`#fdf5e0`) en bibliotecas y misiones — el fondo oscuro dificulta la lectura.
- Videos: nunca `?wmode=opaque` en URLs de YouTube (Error 153 en CREA).
- Botones de navegación: NO agregar "siguiente misión" ni "volver" entre páginas de misiones.
- Material docente: NO publicar sin decisión explícita.
- Estructura: cada subreino autocontenido en su propia carpeta (`s6-`, `s7-`, `s8-`…).

---

## Comandos útiles

```bash
# Ver estado antes de stagear
git status --short

# Agregar archivos específicos (nunca git add -A)
git add README.md ROADMAP.md CHANGELOG.md

# Commit y push
git commit -m "Descripción del cambio"
git push
```
