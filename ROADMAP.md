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

- [x] **Biblioteca S8** — 3 lecciones + hub en `s8-ecuaciones/biblioteca/`. ✓
- [x] **Biblioteca desbloqueada en el mapa** — territorio activo, enlace a `biblioteca/index.html`. ✓
- [x] **Cierre S8 publicado** — `s8-ecuaciones/cierre/` con `index.html`, ficha y resolución. ✓
- [ ] **Habilitar MC-S8** cuando corresponda: `cierre/index.html`, `MC_HABILITADO = false` → `true`.
- [ ] **Habilitar resolución MC-S8** en momento posterior: `RESOLUCION_HABILITADA = false` → `true`.
- [ ] **Habilitar Desafío Final S8 en el mapa** — `s8-ecuaciones/index.html`, territorio `desafio`: `bloqueado: false`, `enlace: "cierre/index.html"`.
- [ ] **Habilitar resoluciones restantes** cuando estén disponibles (E03, E06, E07, E08, E10 aún sin HTML en repo).

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
| Material docente E06/E07 | Versión profe oculta en el sitio | Mantener así |

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
