# Ingeniería de Software Ágil 2
## Universidad ORT Uruguay - Facultad de Ingeniería
## Grupo M7B ID - Obligatorio - Entrega 2
## Santiago Blanco (282654) - Elian Priaron(286556) - Gaston Roig (291873)
---

|Revisado por|Rol|Fecha|Aprobado|
|---|---|---|---|
|Santiago Blanco|Dev./Tester|||
|Elian Priaron|Dev./Tester|||
|Gaston Roig|Product Owner|||

## Registro de Reuniones
|Fecha|Hora|Duración|Asistentes|Objetivo|
|---|---|---|---|---|
|2025-04-26|10:00|2 horas|Santiago Blanco, Elian Priaron, Gaston Roig|Arreglos en conflictos anteriores del código, configuración del pipeline. Discusión y organización de futuros pasos para continuar con el trabajo.|
|2025-04-28|14:00|2 horas|Elian Priaron, Gaston Roig|Continuacion de desarrollo del pipeline y prueba del mismo. Reestructuracion del tablero. Arreglo de dos de las issues, la #10 y la #17.|
|2025-04-29|10:00|2 horas|Santiago Blanco, Elian Priaron, Gaston Roig|Arrego de la issue #2. Agregado de GitHub action para checkpoint en merging a rama develop. Comienzo de la documentación para la segunda entrega.|

## Carga Horaria
|Integrante|Horas Grupal|Horas Individual|
|---|---|---|
|Santiago Blanco|4|0|
|Elian Priaron|6|0|
|Gaston Roig|6|0|
|**Sumatoria (Grupal)**|**4**|*N/A*|

## Cambios Realizados en la estructura del repositorio

- Se agregó la carpeta de workflows para el pipeline de GitHub Actions, dentro de la carpeta `.github`.
- Se borró el archivo .gitignore, ya que no es necesario para el funcionamiento del repositorio, porque ya existen los gitignore en las carpetas de backend y frontend, entregados como consigna.

```
 .
 ├ .git
 ├ .github
 │  ├ workflows
 │  │  ├ ci.yml
 │  │  ├ cd.yml
 │  │  ├ checkpoint.yml
 ├ app
 │  ├ code
 │  │  ├ docker-compose.yml
 │  │  ├ backend
 │  │  ├ frontend
 │  ├ db
 │  │  ├ entrega-1
 │  │  │  ├ empty
 │  │  │  ├ loaded
 │  │  ├ entrega-2
 │  │  │  ├ empty
 │  │  │  ├ loaded
 │  ├ doc
 │  │  ├ consigna
 │  │  ├ entrega-1
 │  │  ├ entrega-2
 │  ├ exports
 │  │  ├ drugsExport1.json
 │  │  ├ drugsExport2.json
 │  │  ├ drugsExport3.json
 ├ entregas
 │  ├ entrega-1
 │  │  ├ README.md
 │  ├ entrega-2
 │  │  ├ README.md
 │  ├ entrega-3
 │  │  ├ README.md
 │  ├ entrega-4
 │  │  ├ README.md
 │  ├ entrega-5
 │  │  ├ README.md
 ├ img
 |  ├ meetings
 |  ├ issues
 |  ├ kanban
 ├ README.md
```

## Cambios en el tablero de Kanban

El primer cambio realizado en el tablero kanban fue la creación de una columna para cada uno de los estados del flujo de trabajo. En este caso, se crearon las siguientes columnas de TDD[Green] y TDD[Refactor]. Estas dos columnas se crearon para especificar detalladamente la etapa en la que nos encontrábamos a la hora de realizar el desarrollo. En un principio se decidió sustituir la columna de Doing por estas dos, pero luego de discutirlo decidimos mantenerla, ya que hay ciertas issues o Tasks que nosotros identificamos que no corresponden a ninguna de las otras columnas mencionadas. Por ejemplo, la issue #2, era cambiar el versionado de la API, y no requería de ningún testeo, por lo que no se puede incluir en la columna de TDD[Green], por lo tanto el flujo de esta issue será: To-Do - Doing - Done. En otros casos será To-Do - TDD[Green] - TDD[Refactor] - Done.

Para observar mejor el flujo de trabajo se dejan imágenes adjuntadas en la carpeta img/kanban.

## Uso de Test Driven Development (TDD) / Desarrollo

En esta entrega no se utilizo TDD, ya que no se realizaron cambios en el codigo del backend que afectaran a las pruebas.

## Issues y Tasks

## Ceremonias para esta entrega
- Retrospective
- Review