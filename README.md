# Reinos Matemáticos 2026
**Proyecto web educativo — 8.º EBI · Liceo de Médanos, Uruguay**
Autora pedagógica: Gabriela Michelle Fernández

---

## 🌐 URL pública (GitHub Pages)

```
https://laprofe2007.github.io/matematica-8ebi/
```

Página de entrada: `index.html` en la raíz.

---

## 🗂️ Estructura de carpetas

```
raíz/
├── index.html                          ← Portal de todos los reinos
├── iconos_web/                         ← Iconos PNG compartidos (castillo, biblioteca, etc.)
├── imagenes para ejercicios/           ← Imágenes educativas (infografías, ilustraciones)
│
├── proporciones/                       ← Reino 1: Razones y Proporcionalidad
│   ├── index.html                      ← Mapa del reino (territorios interactivos)
│   ├── biblioteca.html                 ← Material teórico con videos y teoría
│   ├── Fabrica_Pintura_Applet_v3.html  ← Applet interactivo misión I
│   ├── Ciudad_Proporciones_Interactivo.html ← Applet interactivo misión IV
│   └── Actividades/                    ← PDFs de actividades del reino
│       ├── Prologo_Reino_Razones_Proporciones.pdf
│       ├── TD_Bitacora_Explorador.pdf
│       ├── S4 Act1_Fabrica_Pintura_v3.pdf
│       ├── S4_Act2_Mapa_Uruguay_Escala.pdf
│       ├── S4_Act3_ElIntruso_v2.pdf
│       ├── S4_Act4_CiudadProporciones.pdf
│       ├── S4_Act5_ViajeEgresados_v2.pdf
│       ├── S4_Act6_Clasificacion_v2.pdf
│       ├── Act8_K_en_todos_lados_v2.pdf
│       ├── S4_Mini_Eval_Estudiante_v2.pdf
│       └── EvalIntegradora_S3_S4_v4.pdf
│
└── tierras-sin-mapa/                   ← Reino 2: Probabilidad y Estadística
    ├── index.html                      ← Mapa del reino
    ├── intro.html                      ← Intro animada (frases cinematográficas)
    ├── Simulador_Sobres_Panini2026.html ← Simulador interactivo (C38)
    └── Actividades/                    ← PDFs de actividades del reino
        ├── capitlulo 4 mate porras.pdf ← Material teórico principal
        ├── Control_Lectura_Probabilidad_S5.pdf
        ├── C34_Desafio_Adivinos.pdf
        ├── C36_Gran_Experimento_Dado.pdf
        ├── C37_Dado_y_Moneda.pdf
        ├── C37_Deberes.pdf
        ├── C38_Panini_Figuritas.pdf
        ├── C39_Del_Conteo_a_la_Proporcion.pdf
        ├── C40_Hacia_la_Probabilidad.pdf
        ├── C41_C42_EspacioMuestral_Eventos.pdf
        ├── C43_Del factor k al porcentaje.pdf
        ├── C44_Arbol_Interseccion_Independencia.pdf
        ├── C45_Juegos_de_Azar_5_versiones.pdf
        ├── C46_Evaluacion_Integradora_Probabilidad.pdf
        ├── Probabilidad_en_Contexto.pdf
        └── Viñeta conceptual.png
```

---

## 🔗 URLs directas

| Página | URL |
|---|---|
| Portal (todos los reinos) | `/` |
| Reino Proporciones — mapa | `/proporciones/index.html` |
| Reino Proporciones — biblioteca | `/proporciones/biblioteca.html` |
| Applet Fábrica de Pintura | `/proporciones/Fabrica_Pintura_Applet_v3.html` |
| Applet Ciudad Proporciones | `/proporciones/Ciudad_Proporciones_Interactivo.html` |
| Las Tierras sin Mapa — intro | `/tierras-sin-mapa/intro.html` |
| Las Tierras sin Mapa — mapa | `/tierras-sin-mapa/index.html` |
| Simulador Panini | `/tierras-sin-mapa/Simulador_Sobres_Panini2026.html` |

---

## 🏗️ Arquitectura técnica

- **Tecnología**: HTML + CSS + JS puro. Sin frameworks, sin build tools.
- **Despliegue**: GitHub Pages (rama `main`, carpeta raíz).
- **Fuentes**: Cinzel (títulos) + Libre Baskerville (cuerpo) — Google Fonts.
- **Nuevo reino**: crear carpeta `nombre-reino/` con su `index.html` y `Actividades/`, luego agregar tarjeta en `index.html` raíz.

### Mapa de reino (index.html de cada reino)
- SVG cartográfico con territorios posicionados con `--x` / `--y` CSS vars
- Array JS `territorios[]` controla nombre, icono, posición, enlace y tipo de modal
- Sistema de modales: detalle (para PDFs/páginas) + actividades (lista con scroll) + evaluación (bloqueada) + simulador GeoGebra (en tierras-sin-mapa)
- Focus trap + Escape key + click en backdrop para cerrar modales
- Responsive: posiciones desktop/mobile en cada territorio

### Paleta de colores
**Portal y biblioteca** (fondo claro):
```css
background: #fdf5e0   /* pergamino claro */
--ink:   #2a1c12      /* texto principal */
--gold:  #8a5e14      /* subtítulos, bordes */
--amber: #7a4f0a      /* títulos h1/h2 */
```

**Mapas de reinos** (fondo cálido dorado):
```css
background: #f2e2b0   /* pergamino dorado */
```

**Tierras sin Mapa** (fondo oscuro):
```css
background: #0D1B2A   /* azul noche */
--gold:  #D4A017      /* dorado brillante */
```

---

## ⚠️ Reglas de diseño (no cambiar)

- Fuentes: siempre Cinzel + Libre Baskerville
- Biblioteca y portal: fondo CLARO — el oscuro hace ilegible el texto
- Videos YouTube: nunca usar `?wmode=opaque` — causa Error 153
- Imágenes: hospedar en el repo, nunca URLs de Ceibal/Schoology (requieren login)
- Cada reino: su propia carpeta con todo adentro
- `index.html` raíz: solo navegación entre reinos, sin actividades ni teoría

---

## 📋 Estado actual (junio 2026)

| Reino | Estado |
|---|---|
| Proporciones | ✅ Completo y publicado |
| Las Tierras sin Mapa (Probabilidad) | ✅ Completo y publicado |
| Siguientes reinos | 🔒 Placeholder en portal, se agregan durante el año |

---

## Actualización julio 2026

El enlace principal para CREA sigue siendo:

```text
https://laprofe2007.github.io/matematica-8ebi/
```

Estado actualizado:

| Reino | Estado julio 2026 |
|---|---|
| Proporciones | Publicado, con misiones, biblioteca, applets, bitácora y desafío habilitado |
| Las Tierras sin Mapa | Publicado, con intro, biblioteca, actividades C34-C46, GeoGebra y simulador Panini |
| Siguientes reinos | Pendientes de creación durante el curso |

Notas de mantenimiento:

- El desafío del Reino de las Proporciones ya está habilitado para estudiantes.
- La mini-evaluación y la evaluación integradora de Proporciones están enlazadas desde el modal Desafío.
- El Reino Las Tierras sin Mapa mantiene su carpeta propia con `index.html`, `intro.html`, `Simulador_Sobres_Panini2026.html` y `Actividades/`.
- Si se reemplaza un PDF manteniendo el mismo nombre, alcanza con agregar, commitear y subir ese archivo.
- Material docente o borradores no deben mostrarse en el sitio salvo decisión explícita.

Ver también: [`ROADMAP.md`](ROADMAP.md).
