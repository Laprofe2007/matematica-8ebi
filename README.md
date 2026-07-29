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

## 📋 Estado actual (julio 2026)

| Reino | Estado |
|---|---|
| Proporciones | ✅ Completo y publicado |
| Las Tierras sin Mapa (Probabilidad) | ✅ Completo y publicado |
| Álgebra y las Funciones | ✅ Completo — 6 misiones, biblioteca y cierre activos |
| Siguientes reinos | 🔒 Placeholder en portal, se agregan durante el año |

---

## Estructura completa de carpetas (julio 2026)

```
raíz/
├── index.html                                  ← Portal de todos los reinos
├── iconos_web/                                 ← Iconos PNG compartidos
├── imagenes para ejercicios/                  ← Imágenes educativas
│
├── proporciones/                               ← Reino 1: Razones y Proporcionalidad
│   ├── index.html
│   ├── biblioteca.html
│   ├── Bitacora_Cierre_Proporcionalidad.html
│   ├── Fabrica_Pintura_Applet_v3.html          ← Applet activo (contenido v4)
│   ├── Ciudad_Proporciones_Interactivo.html
│   └── Actividades/                            ← 11 PDFs
│
├── tierras-sin-mapa/                           ← Reino 2: Probabilidad y Estadística
│   ├── index.html
│   ├── intro.html
│   ├── Simulador_Sobres_Panini2026.html
│   └── Actividades/                            ← 15 PDFs + 1 imagen
│
└── algebra-funciones/                          ← Reino 3: Álgebra y las Funciones
    ├── index.html                              ← Mapa del reino (5 territorios activos + 3 placeholders)
    ├── prologo/
    │   └── index.html                          ← Crónica "El misterio del número sin nombre"
    ├── biblioteca/
    │   ├── index.html                          ← Índice de lecciones
    │   ├── leccion1_variables_expresiones.html
    │   ├── leccion2_lenguaje_algebraico.html
    │   ├── leccion3_terminos_semejantes.html
    │   ├── leccion4_monomios_polinomios.html   ← Monomio, coeficiente, semejantes, valor numérico
    │   └── actividad4_definiciones.pdf         ← PDF descargable de la Lección 4
    ├── misiones/
    │   ├── mision-01/  ← A-01 Las letras que ya conocíamos (PNG)
    │   ├── mision-02/  ← A-02 Una escritura para cualquier figura (PDF)
    │   ├── mision-03/  ← A-03 El intruso de las expresiones (PDF · Deberes)
    │   ├── mision-04/  ← A-04 Expresiones en acción (PDF)
    │   ├── mision-05/  ← A-05 La tarifa del taxi (PDF)
    │   └── mision-06/  ← A-06 Perímetros con letras (PDF)
    └── cierre/
        ├── index.html                          ← Gateway con MC_HABILITADO y RESOLUCION_HABILITADA
        ├── mc_s6_actividades.html              ← Mini control interactivo (v2)
        ├── mc_s6_resolucion_explicada.html     ← Resolución comentada (bloqueada por separado)
        └── mc_s6_resolucion_explicada.pdf      ← PDF descargable de la resolución
```

---

## Notas de mantenimiento

- El desafío del Reino de las Proporciones ya está habilitado para estudiantes.
- La mini-evaluación y la evaluación integradora de Proporciones están enlazadas desde el modal Desafío.
- **Habilitar el mini control MC-S6**: en `algebra-funciones/cierre/index.html` cambiá `const MC_HABILITADO = false` por `true` y hacé push.
- **Habilitar la resolución explicada** (momento posterior): en el mismo archivo cambiá `const RESOLUCION_HABILITADA = false` por `true` y hacé push. Son independientes.
- La Misión III (A-03) está rotulada como "Deberes" en el modal y en su página visor.
- Si se reemplaza un PDF manteniendo el mismo nombre, alcanza con agregar, commitear y subir ese archivo.
- Material docente o borradores no deben mostrarse en el sitio salvo decisión explícita.
- `Fabrica_Pintura_Applet_v4.html` existe solo en la PC local — reservado para el reino de Funciones Lineales.

Ver también: [`ROADMAP.md`](ROADMAP.md).
