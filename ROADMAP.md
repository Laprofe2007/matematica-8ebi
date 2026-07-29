# Roadmap - Reinos Matematicos 2026

Este archivo resume el estado y las proximas decisiones del proyecto.

## Enlace publico principal

```text
https://laprofe2007.github.io/matematica-8ebi/
```

Ese enlace debe mantenerse estable porque puede estar publicado en CREA y otros documentos.

## Reinos publicados

### Reino de las Proporciones

Estado: publicado y funcional.

Incluye:

- Prologo narrativo.
- Biblioteca teorica.
- Misiones del explorador.
- Applet Fabrica de Pintura.
- Applet Ciudad de las Proporciones.
- Bitacora del explorador.
- Act 8 - K en todos lados.
- Desafio habilitado:
  - Minievaluacion.
  - Evaluacion Integradora.

Pendientes posibles:

- `proporciones/Fabrica_Pintura_Applet_v4.html` — reservado para el reino de Funciones Lineales. Cuando se trabaje esa unidad, publicarlo como applet de ejemplo de recta y = kx. No publicar aun.
- Decidir si la hoja docente de correccion de la evaluacion integradora debe subirse como respaldo interno o mantenerse fuera del sitio publico.

### Las Tierras sin Mapa

Estado: publicado y funcional.

Incluye:

- Intro animada.
- Opcion de lectura completa del prologo.
- Biblioteca con material teorico y control de lectura.
- Actividades C34 a C46.
- Simulador de dados con GeoGebra.
- Simulador Panini.
- Evaluacion del reino preparada para habilitar cuando corresponda.

Pendientes posibles:

- Revisar periodicamente peso de PDFs e imagenes.
- Habilitar o ajustar evaluaciones segun avance del curso.

### Reino del Algebra y las Funciones

Estado: publicado y funcional (julio 2026).

Incluye:

- Prologo narrativo: cronica "El misterio del numero sin nombre".
- Biblioteca: 4 lecciones interactivas (variables y expresiones, lenguaje algebraico, terminos semejantes, monomios y definiciones clave). Leccion 4 incluye PDF descargable.
- Misiones I a VI: fichas A-01 (PNG) y A-02 a A-06 (PDF con visor embed + descarga). Mision III rotulada como Deberes.
- Cierre: gateway `cierre/index.html` con dos toggles independientes:
  - `MC_HABILITADO = false` — controla el acceso al mini control interactivo.
  - `RESOLUCION_HABILITADA = false` — controla la resolucion explicada (HTML + PDF descargable).
- Mapa del reino: 5 territorios activos + 3 placeholders bloqueados (S7, S8, S9) para secuencias futuras.

Pendientes:

- Habilitar MC-S6: editar `MC_HABILITADO = false` → `true` y hacer push.
- Habilitar resolucion: editar `RESOLUCION_HABILITADA = false` → `true` y hacer push (momento posterior).
- Agregar bitacora PDF cuando este lista (carpeta `bitacora/` existe, sin contenido aun).
- Rellenar contenido de S7, S8, S9 cuando corresponda (territorios ya planeados en el mapa).

## Proximas etapas sugeridas

1. Habilitar MC-S6 en Algebra y Funciones cuando corresponda.
   - Editar `algebra-funciones/cierre/index.html`: cambiar `MC_HABILITADO = false` por `true`.
   - Commit y push. Sin mas cambios necesarios.

2. Agregar bitacora al Reino de Algebra y Funciones.
   - Crear `algebra-funciones/bitacora/index.html` con la pregunta guia y el PDF cuando este listo.

3. Crear nuevos reinos (Geometria, Funciones Lineales, etc.).
   - Crear carpeta propia.
   - Crear `index.html` con el mapa del reino.
   - Agregar tarjeta en portal raiz `index.html`.
   - El applet `proporciones/Fabrica_Pintura_Applet_v4.html` (solo en PC local) es candidato para el reino de Funciones Lineales como ejemplo de recta y = kx.

## Convenciones de trabajo

- Cada reino debe vivir en su propia carpeta.
- Los recursos de cada reino deben estar dentro de su carpeta, preferentemente en `Actividades/`.
- PDFs de estudiantes pueden estar enlazados desde el sitio.
- Material docente solo debe publicarse si se decide explicitamente.
- Antes de mover archivos, revisar enlaces relativos.
- Cambios importantes deben terminar con commit claro y push a `main`.

## Comandos utiles

```powershell
git status --short
git add README.md ROADMAP.md
git commit -m "Actualiza documentacion del proyecto"
git push
```
