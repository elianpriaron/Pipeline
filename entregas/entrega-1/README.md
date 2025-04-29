# Ingeniería de Software Ágil 2
## Universidad ORT Uruguay - Facultad de Ingeniería
## Grupo M7B ID - Obligatorio - Entrega 1
## Santiago Blanco (282654) - Elian Priaron(286556) - Gaston Roig (291873)
---

|Revisado por|Rol|Fecha|Aprobado|
|---|---|---|---|
|Santiago Blanco|Dev./Tester|2025-04-21|✅|
|Elian Priaron|Product Owner|2025-04-21|✅|
|Gaston Roig|Dev./Tester|2025-04-21|✅|

## Registro de Reuniones
|Fecha|Hora|Duración|Asistentes|Objetivo|
|---|---|---|---|---|
|2025-04-04|11:20|1 hora 30 minutos|Santiago Blanco, Elian Priaron, Gaston Roig|Conversación sobre el trabajo y creación del repositorio en GitHub, análisis previo para instalar el obligatorio.|
|2025-04-05|10:00|1 hora 30 minutos|Santiago Blanco, Elian Priaron, Gaston Roig|Clonación del repositorio en los locales de los integrantes, instalación del mismo y prueba de corrida de docker.|
|2025-04-07|18:30|2 horas|Santiago Blanco, Elian Priaron, Gaston Roig|Comienzo del readme, su estructura y definiciones principales requeridas por la letra del trabajo para la primer entrega.|
|2025-04-09|13:00|2 horas|Santiago Blanco, Elian Priaron, Gaston Roig|Reestructura de directorios, traslado al nuevo repositorio, continuación de la documentación y comienzo de identificación de la Deuda Técnica.|
|2025-04-14|09:00|1 hora 30 minutos|Santiago Blanco, Elian Priaron, Gaston Roig|Discusión sobre issues agregadas, y revisión primaria del documento.|
|2025-04-21|12:00|2 horas|Santiago Blanco, Elian Priaron, Gaston Roig|Revisión y finalización de la primera entrega|

## 0. Definición del Marco de Trabajo en Kanban

### Ceremonias a lo largo del proyecto
- Daily: Reunión de corta duración (15 minutos) para revisar el estado de las tareas y coordinar el trabajo del día. Se realizará previo a los encuentros del equipo, y no tiene un horario fijo.

- Reuniones de planificación: Reuniones al inicio de cada entrega para planificar el trabajo y definir las tareas a realizar. Se realizará al inicio de cada entrega.

- Reuniones de revisión (Review): Reuniones al final de cada entrega para revisar el trabajo realizado y presentar los resultados. Se realizará al finalizar cada entrega.

- Retrospectiva: Reunión al final de cada entrega para revisar el trabajo realizado y discutir posibles mejoras en el proceso. Se realizará al finalizar cada entrega.

### Roles para esta entrega
- Product Owner: Elian Priaron. Se encargará de definir los requisitos del proyecto y de la toma de decisiones estratégicas, así como la coordinación del equipo en esta instancia.
- Dev./Testers: Santiago Blanco y Gaston Roig. Se encargarán del desarrollo en esta instancia, que al no involucrar código, será exclusivamente la documentación.

### Metodología de trabajo
Se utilizará la metodología Kanban para la gestión del proyecto. Se utilizará un tablero Kanban para visualizar el flujo de trabajo y gestionar las tareas. El equipo se reunirá con frecuencia para revisar el estado de las tareas y coordinar el trabajo del día.
Las reuniones se llevarán a cabo de forma remota a través de Discord, y cuando se considere necesario por los miembros del equipo, se realizarán reuniones presenciales.
El encargado de la coordinación y fijación del horario de las reuniones en las que participe todo el equipo, va a ser el Product Owner. Se cuenta con un canal de comunicación por grupo de Whatsapp para esto. En otras reuniones específicas, se coordinará en cada caso por los integrantes.

### Definition of Done propuesta
*Esta Definition of Done se aplicará para tickets de desarrollo (en este contexto representadas como Issues), a diferencia de cursos anteriores en donde su ámbito de aplicación eran las Historias de Usuario.*

Siguiendo lo trabajado en el curso y en materias anteriores, aplicándolo a la resolución de tickets y teniendo en cuenta la aplicación del marco Kanban en el que se está trabajando, la Definition of Done para esta entrega es la siguiente:

- El problema que se explica en el issue fue resuelto, o su impacto fue mitigado lo suficientemente como para que no afecte al funcionamiento del sistema.
- El código fue subido a la rama correspondiente.
- El código fue revisado por al menos un miembro del equipo, de forma independiente al autor del commit.
- El código fue testeado y se verificó que no haya errores en la funcionalidad, corriendo todas las pruebas correspondientes.
- El arreglo fue documentado de forma adecuada, siguiendo los estándares de documentación del equipo.
- El código fue aprobado por el encargado del equipo.

## 1. Definición del Proceso de Ingeniería

### Formato del Tablero Kanban y definición de cada uno de los estados.
El tablero será realizado en GitHub, utilizando la herramienta de proyectos. Se utilizarán las siguientes columnas:

- To-Do: Tareas pendientes por realizar.
- Doing: Tareas en progreso.
- Done: Tareas finalizadas.

### __Foto del tablero Kanban__
![Tablero Kanban](img/Tablero_Entrega1_1.png)

### Justificación del Formato
Para el comienzo del proyecto, se eligió usar únicamente esas tres columnas, debido a que sería innecesario tener adicionales en esta primera etapa, ya que no se está desarrollando código. Somos conscientes que a futuro se tienen que agregar nuevas columnas, por ejemplo, expandir la columna de Doing en varias que sean más explicativas, y agregar más columnas tales como TDD y BDD, con esto se logrará perfeccionar el flujo de trabajo, a medida de que se vayan aprendiendo nuevas prácticas del curso y se vayan incorporando nuevas tareas.

## 2. Configuración del Repositorio en GitHub
### Configuración inicial
Se clonó el repositorio creado automáticamente por GitHub Classroom para el equipo. Se creó un README.md para documentar el trabajo realizado. Los fuentes del código se bajaron de Aulas, así como el docker compose y demás documentación del trabajo originalmente de Diseño II.

### Estrategia de Branching
Elegimos hacer uso de la estrategia tradicional de GitFlow, con una rama main (o master) que es en la que se encuentra cada entrega luego de realizada, y una rama develop en la que se van realizando los cambios y desarrollos que aún no fueron entregados oficialmente o que precisan la aprobación de los integrantes del equipo. Asimismo, se tiene una rama por cada entrega en la cual se hacen los commits de documentación, pudiéndose crear más ramas para funcionalidades de código, fixes, etc, en caso de ser necesario. 

### Estándares de Nomenclatura
Para esta entrega, se definieron y utilizaron las ramas de la siguiente manera:

*main*: Rama maestra del proyecto.

*develop*: Rama de desarrollo del proyecto.

*entrega-<#>*: Rama para cada una de las entregas específicas. Se sustituye el placeholder <#> por el número de entrega correspondiente.

*feature/\<nombre_feature\>*: Rama para cada una de las funcionalidades específicas que se vayan a desarrollar. Especialmente se usará en entregas más adelante para cosas relacionadas a código. Se sustituye el placeholder \<nombre_feature\> por el nombre de la funcionalidad correspondiente.

*fix/\<nombre_bug\>*: Rama para cada uno de los fixes que se vayan a realizar. Al igual que el punto anterior se usará en entregas próximamente para arreglos del código. Se sustituye el placeholder \<nombre_bug\> por el nombre del error encontrado correspondiente.

### Archivos & Directorios
Se reorganizaron los archivos y directorios los cuales quedaron en el siguiente formato, que en este caso representamos con un árbol, en el cual también se puede ver la complejidad y organización de cada parte:

```
 .
 ├ .git
 ├ .gitignore
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
 ├ README.md
```

Lo que se hizo fue normalizar la nomenclatura que en el zip entregado no era adecuada ni prolija, se estableció un formato en minúscula para el nombre de las carpetas, siendo cada nombre escrito en inglés, manteniendo en español únicamente los nombres de las entregas. Se eliminaron carpetas innecesarias (Material)y se reestructuró el directorio en orden para que sea más fácil de entender y navegar.  Se creó una carpeta de entregas para guardar las entregas realizadas, en formato de Readme. En este último caso, lo que se hará será mantener el Readme de la última entrega en la raíz del repositorio como una copia con su correspondiente carpeta de imágenes, y todos los otros serán colocados en sus carpetas.

En la entrega final, el README.md que se encuentra en la raíz, será el Informe Académico Final, y el resto de los README.md de las entregas estarán en sus respectivas carpetas. En cada entrega se irán agregando imágenes y documentación que se considere relevante para la entrega.

Con respecto a los respaldos y a la inclusión o no de archivos y directorios en el repositorio, se respaldará e incluirá en el mismo todos los archivos del proyecto, excepto lo definido en el archivo Git Ignore. Este archivo se crea para evitar conflictos con archivos innecesarios que no son parte del proyecto, como por ejemplo archivos temporales, de configuración de los IDE que usamos para el desarrollo, los archivos .env, los DS Store de Mac, etc. Además se ignoran los node_modules del frontend, ya que eso se resuelve localmente en cada máquina con npm. 

El tener la información en el repositorio y hacer commits frecuentes ya nos garantiza que esté respaldada en caso de que se dañe alguna de las máquinas de los miembros del equipo.

## 3. Análisis de la Deuda Técnica & Gestión de la Calidad

### Modelo de Calidad
A continuación se definen los atributos de calidad que se van a utilizar para evaluar el proyecto. Se han elegido los atributos de calidad más relevantes para el proyecto en nuestra opinión, viendo lo que se podrá mejorar en futuras entregas y lo que se considera más importante para el mismo.

### Atributos de calidad escogidos y justificación
- **Seguridad**: Se refiere a la protección de los datos y la información del sistema. Es importante garantizar que el sistema sea seguro y que los datos estén protegidos contra accesos no autorizados. Además es muy importante que se prevengan ataques ya que el sistema va a estar expuesto a internet. Se considera un atributo de calidad importante ya que el sistema va a manejar datos sensibles y es necesario garantizar la privacidad y la seguridad de los mismos. Ejemplos de cosas a prevenir son: Inyecciones SQL, Cross-Site Scripting (XSS), Cross-Site Request Forgery (CSRF), etc.

- **Mantenibilidad**: Se refiere a la facilidad con la que se puede mantener y actualizar el sistema. Es importante garantizar que el sistema sea fácil de mantener y que se puedan realizar cambios y actualizaciones de forma sencilla, con el menor impacto posible ya que sabemos que cuanto más tiempo lleve se traduce en más costos para la empresa. Se considera un atributo de calidad importante ya que el sistema va a estar en constante evolución (clave en DevOps). Ejemplos de cosas a tener en cuenta son: Clean Code, Documentación del código, pruebas automatizadas, patrones, etc.

- **Usabilidad**: Se refiere a la facilidad con la que los usuarios pueden utilizar el sistema, y que el mismo ande correctamente en todos los aspectos. Es importante garantizar que el sistema sea fácil de usar y que los usuarios puedan realizar sus tareas de forma sencilla y eficiente, y que las puedan realizan en sí. Se considera un atributo de calidad importante ya que el sistema va a ser utilizado por personas que no son necesariamente expertas en tecnología. Ejemplos de cosas a tener en cuenta son: Disponibilidad de las funcionalidades del sistema, su funcionamiento correcto, Interfaz, accesibilidad, etc.

- **Funcionalidad**: Se refiere a la capacidad del sistema para cumplir con los requisitos funcionales definidos previamente y necesidades de los usuarios. Es importante garantizar que el sistema cumpla con las expectativas de los usuarios y que se puedan realizar las tareas necesarias de forma eficiente. Se considera un atributo de calidad importante ya que el sistema va a ser utilizado por personas que no son necesariamente expertas en tecnología. Ejemplos de cosas a tener en cuenta son: Disponibilidad de las funcionalidades del sistema, su funcionamiento correcto, Interfaz, accesibilidad, etc.

### Análisis de la Deuda Técnica del Proyecto
En base a las issues reportadas, a continuación se menciona la deuda técnica que posee el proyecto que nos fue entregado.

La deuda técnica de mantenibilidad se refleja en decisiones tomadas por quienes hicieron el codigo, como la utilización de una única interfaz de repositorio para toda la capa de persistencia, la falta de versionado en los endpoints y la presencia de condicionales excesivamente anidados y funciones extensas que complican el refactoring y la escalabilidad. 

Asimismo, yendo a la parte de seguridad, tiene prácticas inseguras como el almacenamiento de contraseñas en texto plano, el uso de excepciones genéricas que complican el control de errores y formas de escribir rutas en el navbar que permiten saltarse mecanismos de autenticación, exponiendo datos sensibles y la seguridad de la pagina.

En el ámbito de la usabilidad, el sistema muestra errores en la interfaz de usuario y en el flujo de interacción: elementos como botones sin funcionalidad, rutas no autoexplicativas y mensajes de error que persisten tras corregir la entrada van a afectar la eficiencia de quienes lo usan. 

Por último, en cuanto a la funcionalidad, el sistema presenta problemas y errores en cuanto a las funcionalidades ya implementadas, por ejemplo invitar a un usuario a una farmacia inexistente. Esto puede llevar a errores en la ejecución de tareas y a una mala experiencia del usuario.

Para superar esta deuda técnica del software de la farmacia, es necesario un diseño modular y coherente de la UX, reforzar las prácticas de seguridad y adoptar patrones arquitectónicos que faciliten tanto el desarrollo futuro como la experiencia del usuario.

## 4. Definición de Issues & Clasificación

### Definición de Issues
Se define a una issue como una tarea o un problema que debe ser resuelto en el proyecto. Las issues se utilizarán para gestionar las tareas del proyecto y para realizar un seguimiento del progreso del mismo. Cada issue tendrá una descripción clara y concisa del problema o la tarea a realizar. Las issues se asignarán a los miembros del equipo según su disponibilidad y habilidades. Cuando el o los responsables de arreglar el problema hayan terminado su trabajo, se deberá revisar el cumplimiento del mismo por parte de otra persona, y finalmente será aprobado por el encargado del equipo.

### Categorización de Issues
Se utilizarán las issues de GitHub para gestionar las tareas del proyecto. Se utilizarán las siguientes etiquetas:

- High: Tareas importantes que deben ser realizadas de la forma más urgente posible. (Color en Github: rojo)
- Medium: Tareas de prioridad media que deben ser realizadas pero no son urgentes, si bien el beneficio de realizarlas es alto. (Color en Github: amarillo)
- Low: Tareas de baja prioridad que pueden ser realizadas sin apuro, ya que su impacto es bajo. (Color en Github: verde)

## 5. Reuniones de Retrospectiva & Review

### Reunión de Retrospectiva
En esta primera entrega se decidió no realizar una reunión de retrospectiva, ya que no se considera necesario, esto se debe a la falta de desarrollo de código y la falta de implementación de tecnologías como para poder aplicar mejoras. Se espera que en las próximas entregas se realicen reuniones de retrospectiva para revisar el trabajo realizado y discutir posibles mejoras en el proceso.

### Reunión de Review
Se realizó una reunión de al final de la entrega para revisar el trabajo realizado y presentar los resultados al PO. En esta reunión se revisaron las issues creadas, analizando tanto las descripciones de cada una de ellas, como la severity y compromises. 
