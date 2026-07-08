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

## Proximas etapas sugeridas

1. Consolidar Proporciones.
   - Confirmar version definitiva del applet de Fabrica de Pintura.
   - Mantener activos solo los enlaces visibles para estudiantes.

2. Consolidar Probabilidad.
   - Revisar actividades en CREA contra los enlaces de GitHub Pages.
   - Mantener simuladores visibles y faciles de abrir.

3. Crear nuevos reinos.
   - Definir tema.
   - Crear carpeta propia.
   - Crear `index.html`.
   - Crear `Actividades/`.
   - Agregar tarjeta en portal raiz.

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
