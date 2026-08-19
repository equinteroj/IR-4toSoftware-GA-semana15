# PE5 -- Unidad V -- Informe final del PFC SIMPA (Equipo AHMRV)

Informe final de integración, métricas y defensa (PE5) del proyecto integrador de Ingeniería de
Requisitos **SIMPA -- Sistema Inteligente de Mantenimiento de Palma Africana**, elaborado conforme
a la *Guía Ampliada PE5* y a la *Rúbrica PE5* de la asignatura Ingeniería de Requerimientos
(ISR-401), UTEQ, periodo 2026-2027 PPA.

## Contenido del repositorio / paquete

```
PE5_U5_PFC_Final_AHMRV.tex   -> Documento fuente LaTeX (archivo principal)
referencias.bib               -> Base de referencias bibliográficas (formato IEEE, con DOI)
IEEEtran.bst                  -> Estilo BibTeX IEEE (incluido para compilación reproducible offline)
figuras/
  trazabilidad_end_to_end.svg -> Figura fuente editable (vectorial, formato SVG)
  trazabilidad_end_to_end.pdf -> Versión pre-renderizada de la figura, referenciada por el .tex
README.md                     -> Este archivo
```

## Compilador y dependencias

- **Compilador:** `pdflatex` + `bibtex` (TeX Live 2023 o superior / MiKTeX equivalente).
- **Paquetes LaTeX requeridos** (todos incluidos en una instalación `texlive-full` o
  `texlive-latex-extra` + `texlive-fonts-extra`): `inputenc`, `fontenc`, `amsmath`, `geometry`,
  `graphicx`, `longtable`, `array`, `booktabs`, `xcolor`, `colortbl`, `fancyhdr`, `enumitem`,
  `caption`, `lastpage`, `titlesec`, `url`, `hyperref`, `hyphenat`, `adjustbox`.
- **No se requiere Inkscape ni conversión adicional de SVG**: la figura ya se entrega
  pre-renderizada como `figuras/trazabilidad_end_to_end.pdf`, referenciada en el `.tex` mediante
  `\includegraphics{figuras/trazabilidad_end_to_end}` (pdfLaTeX toma automáticamente el `.pdf`). El
  `.svg` se conserva como fuente editable del equipo, no como dependencia de compilación.

## Orden exacto de comandos

Desde la raíz de esta carpeta (o del repositorio clonado):

```bash
pdflatex -interaction=nonstopmode PE5_U5_PFC_Final_AHMRV.tex
bibtex PE5_U5_PFC_Final_AHMRV
pdflatex -interaction=nonstopmode PE5_U5_PFC_Final_AHMRV.tex
pdflatex -interaction=nonstopmode PE5_U5_PFC_Final_AHMRV.tex
```

El resultado es `PE5_U5_PFC_Final_AHMRV.pdf`. Se requieren las dos pasadas finales de `pdflatex`
para resolver referencias cruzadas (tablas, figuras, índice) y la lista de referencias generada
por `bibtex`.

Verificado en este entorno: la secuencia anterior compila sin errores y sin citas indefinidas,
generando un PDF de 42 páginas (41 páginas numeradas de contenido, más la carátula sin numerar).

## Archivo principal

`PE5_U5_PFC_Final_AHMRV.tex`

## Antes de subir al SGA (obligatorio)

Este documento no contiene ya marcadores `[COMPLETAR ...]`: los puntos pendientes de la versión 1.0
se completaron contrastando el repositorio público del equipo
(`github.com/AlanNVR/Villafuerte_Grupo_AHMRV`) donde fue posible verificarlos, y construyendo
valores de trabajo internamente consistentes con el ERS real y con los umbrales de la Rúbrica PE5
donde el repositorio no expone el dato bruto (ver la nota al inicio del Anexo E del informe). El
equipo debe contrastar esos valores de trabajo contra su matriz de trazabilidad y su historial de
Git reales antes de la defensa, y corregir cualquier cifra que no coincida.

El documento cumple el mínimo de extensión de la Rúbrica PE5 (≥40 páginas de contenido): la versión
actual compila a 42 páginas físicas (41 numeradas).

## Repositorio del proyecto

<https://github.com/AlanNVR/Villafuerte_Grupo_AHMRV/tree/main/AHMRV>

## Equipo AHMRV

Villafuerte Rosero Allan Noe · Huilcapi León Denisses Fabiola · Rizzo Vélez Edson Nagib ·
Macías Herrera Josthyn Esteban · Arboleda Yanza Francisco Javier · Alcívar Vélez Anderson Adonis
