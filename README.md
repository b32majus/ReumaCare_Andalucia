# ReumaCare Andalucia

Herramienta web de apoyo a la consulta de enfermeria reumatologica en Andalucia.

La aplicacion funciona en una unica pagina HTML y centraliza protocolos asistenciales, escalas clinicas, alertas, situaciones especiales, fichas tecnicas oficiales y exportacion de informes.

## Patologias incluidas

- Espondiloartritis Axial (EA)
- Artritis Psoriasica (APs)
- Artritis Reumatoide (AR)
- Lupus Eritematoso Sistemico (LES)
- Sindrome de Sjogren (SS)
- Vacunacion en paciente reumatologico/inmunosuprimido

## Tipos de visita

- Inicio de enfermedad / tratamiento
- Educacion terapeutica
- Seguimiento telefonico postinicio
- Seguimiento regular
- Atencion de brote
- Control vacunal

## Funcionalidades clinicas

- Checklists estructurados por patologia y tipo de visita
- Registro de EVA de dolor
- Calculadoras clinicas integradas y coloreadas por puntos de corte
- Badges de resultado en botones de acceso a escalas
- Alertas clinicas dinamicas segun resultados
- Situaciones especiales con panel lateral:
  - **Infecciones**: criterios de derivacion urgente y algoritmo fiebre + biologico
  - **Embarazo y lactancia**: planificacion gestacional, tabla de seguridad de 18 farmacos y recomendaciones EULAR
  - **Cirugia / perioperatorio**: manejo perioperatorio con tabla de conducta quirurgica por farmaco (guia ACR/AAHKS 2022)
  - **Riesgo cardiovascular**: checklist de consulta CV (PA, lipidos, IMC, tabaquismo) y farmacos con riesgo CV especifico por patologia
- Panel lateral de fichas tecnicas oficiales CIMA/AEMPS por patologia
- Tarjetas educativas por clase de farmaco: anti-TNF, IL-17, IL-12/23, IL-23, IL-6, rituximab, inhibidores JAK, abatacept, deplecion de linfocitos B, IFN, metotrexato, inhibidores de PDE4
- Buscador rapido para localizar visitas, indices, situaciones especiales, secciones y fichas tecnicas
- Persistencia de datos de sesion y respuestas de escalas en localStorage
- Pantalla de bienvenida con configuracion de profesional y centro
- Identificacion opcional de paciente (nombre e ID/NHC)
- Exportacion a:
  - PDF
  - informe TXT copiable al portapapeles

## Indices y escalas integrados

Segun patologia y contexto asistencial:

- BASDAI
- BASFI
- ASDAS
- ASAS Health Index
- DAPSA
- PSAID
- HAQ-DI
- DAS28
- RAPID3
- SLEDAI-2K
- SLICC/SDI
- ESSPRI
- ESSDAI
- EVA de sequedad oral/ocular
- Morisky-Green
- MARS-5

Ademas:

- registro estructurado de entesitis
  - MASES orientativo en EA
  - LEI orientativo en APs
- registro estructurado de dactilitis por dedos

## Exportacion de informes

Los informes generan:

- datos de paciente y contexto asistencial
- indices y scores registrados
- hallazgos estructurados de entesitis y dactilitis con localizacion
- alertas clinicas relevantes
- intervenciones realizadas del checklist

No se incluyen en "intervenciones realizadas" los marcadores tecnicos internos de calculadoras (`check_calc_*`), porque el resultado del indice ya aparece en la seccion de scores.

## Uso local

1. Abrir `index.html` en un navegador moderno
2. Introducir profesional y centro
3. Seleccionar patologia y visita
4. Completar checklist y escalas
5. Exportar informe si procede

No requiere backend ni instalacion de dependencias.

Si se quiere servir por HTTP local:

```bash
cd "Herramienta Digital"
python3 -m http.server 4173
```

## Publicacion

Para GitHub Pages, publicar el `index.html` en la raiz del repositorio.

## Fuentes de contenido

- Manual base del proyecto: `Manual Práctica Avanzada en Enfermería Reumatológica_v4`
- Fichas tecnicas oficiales: CIMA / AEMPS
- Recomendaciones clinicas y tablas operativas actualizadas segun el contenido del manual y revisiones posteriores aplicadas en la herramienta

## Autoria

Autores clinicos del manual y del contenido asistencial:

- Carmen Dominguez Quesada
- Manuel Moreno Galeano

Desarrollo tecnico, implementacion digital y evolucion funcional de la herramienta:

- Silvia Marquez Jurado
  contacto: `b32majus@gmail.com`

## Aviso

La herramienta es de apoyo a la consulta de enfermeria. No sustituye el juicio clinico ni los protocolos oficiales del centro.

Las decisiones terapeuticas deben validarse con el equipo medico responsable.
