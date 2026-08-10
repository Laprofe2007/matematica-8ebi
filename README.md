# Reinos Matemáticos 2026

**Proyecto web educativo — 8.º EBI · Liceo de Médanos, Uruguay**
Autora pedagógica: Gabriela Michelle Fernández

---

## URL pública (GitHub Pages)

```
https://laprofe2007.github.io/matematica-8ebi/
```

Esa URL debe mantenerse estable. Puede estar publicada en CREA, Google Classroom u otros documentos compartidos con estudiantes.

---

## Estado actual (agosto 2026)

> Actualización documental 2026-08-10: se alineó este README con el ROADMAP vigente. Propósito: reflejar que MC-S6 y su resolución están habilitadas, que A-12 no forma parte de S7 y que MC-S8 permanece bloqueada. Reversión: `git restore README.md` antes del commit, o revertir el commit correspondiente si ya fue publicado.

| Reino | Subreino | Misiones | Biblioteca | Desafío / MC |
|---|---|---|---|---|
| Proporciones (S3/S4) | — | ✅ A-01 a A-08 | ✅ Con videos | ✅ Habilitado |
| Las Tierras sin Mapa (S5) | — | ✅ C34 a C46 | ✅ Con teoría | 🔒 Pendiente |
| Álgebra y Funciones | S6 — Código de Letras | ✅ A-01 a A-06 | ✅ 4 lecciones | ✅ MC y resolución habilitadas |
| Álgebra y Funciones | S7 — El Mundo de los Polinomios | ✅ A-07, A-08, A-10, A-11 | ✅ 5 lecciones | 🔒 MC bloqueado · resolución bloqueada |
| Álgebra y Funciones | S8 — El Equilibrio Oculto | ✅ E01 a E10 (10 misiones) | ✅ 3 lecciones | 🔒 MC bloqueado · resolución bloqueada |

---

## Interruptores de contenido bloqueado

Para habilitar contenido, editar la constante en el archivo indicado y hacer push. Sin otros cambios.

| Archivo | Constante | Estado actual | Efecto |
|---|---|---|---|
| `algebra-funciones/cierre/index.html` | `MC_HABILITADO` | `true` ✅ | Mini control S6 habilitado |
| `algebra-funciones/cierre/index.html` | `RESOLUCION_HABILITADA` | `true` ✅ | Resolución S6 habilitada |
| `algebra-funciones/s7-polinomios/cierre/index.html` | `MC_HABILITADO` | `false` 🔒 | Bloqueado hasta nueva habilitación |
| `algebra-funciones/s7-polinomios/cierre/index.html` | `RESOLUCION_HABILITADA` | `false` 🔒 | Bloqueado hasta corrección en clase |
| `algebra-funciones/s8-ecuaciones/cierre/index.html` | `MC_HABILITADO` | `false` 🔒 | Bloqueado hasta nueva habilitación |
| `algebra-funciones/s8-ecuaciones/cierre/index.html` | `RESOLUCION_HABILITADA` | `false` 🔒 | Bloqueado hasta corrección en clase |

---

## Estructura de carpetas completa

```
raíz/
├── index.html                                        ← Portal de todos los reinos
├── iconos_web/                                       ← Íconos PNG compartidos (castillo, biblioteca, cofre…)
├── imagenes para ejercicios/                         ← Infografías y materiales visuales
│
├── proporciones/                                     ← Reino 1: Razones y Proporcionalidad
│   ├── index.html                                    ← Mapa del reino
│   ├── biblioteca.html                               ← Material teórico con videos
│   ├── Bitacora_Cierre_Proporcionalidad.html
│   ├── Fabrica_Pintura_Applet_v3.html                ← Applet activo en el sitio
│   ├── Fabrica_Pintura_Applet_v4.html                ← Versión local, NO publicada (ver ROADMAP)
│   ├── Ciudad_Proporciones_Interactivo.html
│   └── Actividades/                                  ← 13 PDFs (estudiante + docente)
│
├── tierras-sin-mapa/                                 ← Reino 2: Probabilidad y Estadística
│   ├── index.html                                    ← Mapa del reino
│   ├── intro.html                                    ← Intro animada con citas cinematográficas
│   ├── Simulador_Sobres_Panini2026.html
│   └── Actividades/                                  ← 16 PDFs + 1 imagen
│
└── algebra-funciones/                                ← Reino 3: Álgebra y las Funciones
    ├── index.html                                    ← Mapa del reino (3 subreinos + placeholders)
    ├── prologo/
    │   └── index.html                                ← "El misterio del número sin nombre"
    │
    ├── biblioteca/                                   ← Biblioteca del reino — vinculada a S6
    │   ├── index.html
    │   ├── leccion1_variables_expresiones.html
    │   ├── leccion2_lenguaje_algebraico.html
    │   ├── leccion3_terminos_semejantes.html
    │   ├── leccion4_monomios_polinomios.html
    │   └── actividad4_definiciones.pdf
    │
    ├── misiones/                                     ← Misiones de S6 (A-01 a A-06)
    │   ├── mision-01/  A-01 Las letras que ya conocíamos (PNG)
    │   ├── mision-02/  A-02 Una escritura para cualquier figura (PDF)
    │   ├── mision-03/  A-03 El intruso de las expresiones (PDF · Deberes)
    │   ├── mision-04/  A-04 Expresiones en acción (PDF)
    │   ├── mision-05/  A-05 La tarifa del taxi (PDF)
    │   ├── mision-06/  A-06 Perímetros con letras (PDF)
    │   └── resoluciones/
    │       ├── A-01_A-02_Resolucion_Explicada.html
    │       ├── A-04_Resolucion_Explicada.html
    │       └── A-05_Resolucion_Explicada.html
    │
    ├── cierre/                                       ← Desafío Final S6
    │   ├── index.html   (MC_HABILITADO=true · RESOLUCION_HABILITADA=true)
    │   ├── mc_s6_actividades.html
    │   ├── mc_s6_resolucion_explicada.html
    │   └── mc_s6_resolucion_explicada.pdf
    │
    ├── s6-codigo-letras/
    │   └── index.html                                ← Mapa del Subreino 1
    │
    ├── s7-polinomios/                                ← Subreino 2: El Mundo de los Polinomios
    │   ├── index.html                                ← Mapa (4 misiones activas · Biblioteca · Desafío 🔒)
    │   ├── biblioteca/
    │   │   ├── index.html                            ← Hub de 5 lecciones
    │   │   ├── Leccion_Suma_Resta_Polinomios.html    Lección 1 — suma y resta en columna
    │   │   ├── leccion-2.html                        Lección 2 — multiplicación · propiedad distributiva
    │   │   ├── Leccion_Multiplicacion_Polinomios.html Lección 3 — multiplicación en columna
    │   │   ├── leccion-4.html                        Lección 4 — cuadrado de un binomio · producto notable
    │   │   ├── leccion-5.html                        Lección 5 — cuadrado de un binomio · versión gráfica
    │   │   ├── pag104_Porras_Leccion.png
    │   │   └── pag107_Producto_Notable_Leccion.pdf
    │   ├── misiones/
    │   │   ├── mision-01/  A-07 Clasificación de polinomios (PDF) · resolución ✅
    │   │   ├── mision-02/  A-08 Suma y resta (PDF) · resolución ✅
    │   │   ├── mision-03/  A-09 Refuerzo suma/resta (PDF+PNG · Deberes · sin misión digital)
    │   │   ├── mision-04/  A-10 Multiplicación (PDF) · resolución ✅
    │   │   ├── mision-05/  [Refuerzo mult, sin código activo · archivos mantenidos]
    │   │   └── mision-06/  A-11 Del rectángulo al cuadrado de un binomio (PDF) · resolución ✅
    │   ├── resoluciones/
    │   │   ├── A07_Clasificacion_Polinomios_Resolucion.html
    │   │   ├── A08_Suma_Resta_Polinomios_Resolucion.html
    │   │   ├── A10_Multiplicacion_Polinomios_Resolucion.html
    │   │   └── A11_Cuadrado_Binomio_Resolucion.html
    │   └── cierre/                                   ← Desafío Final S7
    │       ├── index.html   (MC_HABILITADO=false · RESOLUCION_HABILITADA=false)
    │       ├── mc_s7_polinomios.pdf
    │       └── mc_s7_resolucion_explicada.html
    │
    └── s8-ecuaciones/                                ← Subreino 3: El Equilibrio Oculto
        ├── index.html                                ← Mapa (10 misiones · Biblioteca ✅ · Desafío 🔒)
        ├── biblioteca/
        │   ├── index.html                            ← Hub de 3 lecciones
        │   ├── Biblioteca_L1_Introduccion_a_las_ecuaciones.html  Lección 1 — introducción
        │   ├── Biblioteca_L1_Lenguaje_y_equivalencia.html        Lección 2 — vocabulario y equivalencia
        │   └── Biblioteca_L2_Metodo_de_Polya.html                Lección 3 — método de Polya
        ├── cierre/                                   ← Desafío Final S8
        │   ├── index.html   (MC_HABILITADO=false · RESOLUCION_HABILITADA=false)
        │   ├── MC-S8_ficha.html
        │   └── MC-S8_resolucion.html
        ├── misiones/
        │   ├── mision-01/  E01 — El pijama de la muerte (PNG)
        │   ├── mision-02/  E02 — Método de inversión (PDF) · resolución ✅
        │   ├── mision-03/  E03 — Práctica de ecuaciones (PDF)
        │   ├── mision-04/  E04 — Jo y la consola de juegos (PNG) · resolución ✅
        │   ├── mision-05/  E05 — Ficha interactiva (HTML) · resolución ✅
        │   ├── mision-06/  E11 — Ficha interactiva (HTML) · resolución ✅
        │   ├── mision-07/  E06 — Baraja de ecuaciones (PDF estudiante)
        │   ├── mision-08/  E07 — Bingo de ecuaciones (PDF estudiante)
        │   ├── mision-09/  E08 — Ecuaciones · Freudenthal (PDF)
        │   ├── mision-10/  E09 — Ecuaciones · Porras (PDF · archivado, sin enlace en misiones)
        │   └── mision-11/  E10 — Ecuaciones y problemas · Porras (PDF)
        └── resoluciones/
            ├── E02_resolucion.html
            ├── E04_resolucion.html
            ├── E05_resolucion.html
            └── E11_resolucion.html
```

---

## URLs directas

| Página | Ruta |
|---|---|
| Portal (todos los reinos) | `/` |
| Reino Proporciones — mapa | `/proporciones/index.html` |
| Reino Proporciones — biblioteca | `/proporciones/biblioteca.html` |
| Applet Fábrica de Pintura | `/proporciones/Fabrica_Pintura_Applet_v3.html` |
| Applet Ciudad Proporciones | `/proporciones/Ciudad_Proporciones_Interactivo.html` |
| Las Tierras sin Mapa — intro | `/tierras-sin-mapa/intro.html` |
| Las Tierras sin Mapa — mapa | `/tierras-sin-mapa/index.html` |
| Simulador Panini | `/tierras-sin-mapa/Simulador_Sobres_Panini2026.html` |
| Álgebra y Funciones — mapa | `/algebra-funciones/index.html` |
| S6 — Código de Letras | `/algebra-funciones/s6-codigo-letras/index.html` |
| S6 — Biblioteca | `/algebra-funciones/biblioteca/index.html` |
| S6 — Desafío Final | `/algebra-funciones/cierre/index.html` |
| S7 — El Mundo de los Polinomios | `/algebra-funciones/s7-polinomios/index.html` |
| S7 — Biblioteca | `/algebra-funciones/s7-polinomios/biblioteca/index.html` |
| S7 — Desafío Final (MC-S7) | `/algebra-funciones/s7-polinomios/cierre/index.html` |
| S8 — El Equilibrio Oculto | `/algebra-funciones/s8-ecuaciones/index.html` |

---

## Arquitectura técnica

- **Tecnología**: HTML + CSS + JS puro. Sin frameworks, sin build tools, sin dependencias.
- **Despliegue**: GitHub Pages, rama `main`, carpeta raíz. Push = publicación inmediata.
- **Fuentes**: Cinzel (títulos) + Libre Baskerville (cuerpo) vía Google Fonts. Misiones y resoluciones usan Nunito.
- **Repositorio**: `https://github.com/Laprofe2007/matematica-8ebi`

### Patrón de subreino (cómo funciona el mapa interactivo)

- El `index.html` de cada subreino tiene un array JS `territorios[]` con: nombre, ícono, descripción, posición (desktop/mobile), enlace, estado (bloqueado o no).
- Territorios de tipo `esMisiones: true` abren el modal de misiones (lista con scroll).
- Territorios normales abren un modal de detalle con botón de acción.
- Posicionamiento: `--x` / `--y` CSS custom properties + `transform: translate(-50%, -50%)`.
- Sistema de modales: cierra con Escape, clic en fondo, o botón ×. Focus trap para accesibilidad.
- Responsive: cada territorio tiene posición `desktop` y `mobile` independiente.

### Patrón de cierre / Desafío Final

Cada cierre tiene un `index.html` con dos constantes JS:
```js
const MC_HABILITADO = false;        // Cambiá a true para habilitar el mini control
const RESOLUCION_HABILITADA = false; // Cambiá a true para habilitar la resolución
```
Son independientes. El contenido aparece o se muestra bloqueado según el valor.

### Paleta de colores

**Portal, bibliotecas, misiones, resoluciones** (fondo pergamino claro):
```css
background: #fdf5e0
--ink:   #2a1c12
--gold:  #8a5e14
--amber: #7a4f0a
```

**Mapas de subreinos** (fondo dorado cálido):
```css
background: #f2e2b0 / #f0e0b0
--gold:  #c9983f
--amber: #b07828
```

**Las Tierras sin Mapa** (fondo oscuro noche):
```css
background: #0D1B2A
--gold:  #D4A017
```

**Resoluciones explicadas** (Nunito, fondo lila claro):
```css
background: #f4f2fb
color: #2c1a4d
header: linear-gradient(135deg, #5b2a86, #8e44ad)
```

---

## Reglas de diseño (no cambiar sin revisar)

- Fuentes de subreinos y portal: siempre Cinzel + Libre Baskerville.
- Misiones y resoluciones: Nunito.
- Bibliotecas y portal: fondo CLARO — el oscuro hace ilegible el texto de estudio.
- Videos YouTube: nunca usar `?wmode=opaque` — causa Error 153 en dispositivos CREA.
- Imágenes: alojar en el repositorio. Nunca URLs de Ceibal o Schoology (requieren login).
- Cada subreino: su propia carpeta (`s6-`, `s7-`, `s8-`). Los recursos van adentro.
- Versiones docente / material interno: NO publicar en el sitio sin decisión explícita.
- No agregar botones "volver" ni "siguiente misión" entre páginas de misiones.

---

## Reglas de git para este repositorio

Archivos que **nunca se deben agregar al staging**:

- `proporciones/Fabrica_Pintura_Applet_v4.html` — reservado para reino futuro de Funciones Lineales
- `proporciones/Actividades/hoja docente Correccion a_S3_S4_v4.pdf` — uso interno docente
- `proporciones/Actividades/S4_Act5_ViajeEgresados_v2.pdf` — versión en revisión

---

Ver también: [`ROADMAP.md`](ROADMAP.md) · [`CHANGELOG.md`](CHANGELOG.md)
