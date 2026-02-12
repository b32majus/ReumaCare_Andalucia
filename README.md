# ReumaCare_Andalucia

Herramienta web de apoyo para la consulta de Enfermeria Reumatologica en Andalucia.

ReumaCare_Andalucia centraliza checklists clinicos, escalas de actividad, alertas y exportacion de informes para visitas de inicio, educacion terapeutica, seguimiento, brote y vacunacion.

## Caracteristicas principales

- Protocolos estructurados por patologia: EA, APs, AR, LES y vacunacion.
- Escalas clinicas integradas (segun contexto): BASDAI, BASFI, ASDAS, DAPSA, DAS28, RAPID3, HAQ-DI, PSAID, SLEDAI-2K, ASAS-HI, Morisky y MARS-5.
- Seguimiento telefonico optimizado con escalas aplicables por entrevista.
- Panel de Situaciones Especiales (infecciones, embarazo, cirugia, cardiovascular).
- Exportacion de informe en PDF y copia de informe TXT al portapapeles.
- Interfaz orientada a uso en consulta (desktop-first) y compatible con movil.

## Estructura del proyecto

El proyecto esta implementado como una aplicacion HTML unica:

- `ReumaCare_vKimi_2.html` -> version operativa principal.

Puedes renombrar ese archivo a `index.html` para publicarlo mas facilmente en GitHub Pages.

## Uso local

1. Descarga o clona este repositorio.
2. Abre `ReumaCare_vKimi_2.html` en tu navegador.
3. Introduce profesional/centro en la pantalla de bienvenida.
4. Selecciona patologia y tipo de visita.
5. Completa checklist, escalas y genera informe.

No requiere backend ni instalacion de dependencias.

## Publicacion en GitHub Pages

### Opcion recomendada (archivo raiz)

1. Renombra `ReumaCare_vKimi_2.html` a `index.html`.
2. Sube el repositorio a GitHub.
3. Ve a `Settings` -> `Pages`.
4. En `Build and deployment`, selecciona:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main` (o `master`) y carpeta `/ (root)`
5. Guarda y espera el despliegue.
6. Tu web quedara disponible en la URL de GitHub Pages del repositorio.

### Opcion alternativa (sin renombrar)

Puedes crear un `index.html` minimo que redirija a `ReumaCare_vKimi_2.html`, pero para mantenimiento se recomienda dejar un unico `index.html` principal.

## Privacidad y datos

- La app funciona en cliente (navegador).
- No envia datos a servidor externo por defecto.
- Revisa siempre la politica de privacidad de tu centro antes de uso asistencial.

## Aviso clinico

Esta herramienta es de apoyo a la consulta de enfermeria y no sustituye el juicio clinico ni los protocolos oficiales del centro.

Las decisiones terapeuticas (inicio, suspension o ajuste de tratamiento) deben validarse con el equipo medico responsable.

## Roadmap sugerido

- Mejoras continuas de usabilidad en escritorio.
- Ajustes de contenidos segun protocolos locales.
- Versionado formal de cambios clinicos y funcionales.
