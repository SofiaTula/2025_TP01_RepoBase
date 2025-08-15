Escenario
Recibiste tres tareas clave como parte de un equipo de desarrollo:

Agregar una nueva funcionalidad.
Corregir un error en producción.
Preparar una versión estable del sistema.
Debés organizarte con Git para realizar estas tareas de forma ordenada, trazable y profesional.

Tareas que debés cumplir
1. Configurar tu entorno y preparar tu repositorio
Cloná o forkeá el repositorio base https://github.com/ingsoft3ucc/2025_TP01_RepoBase
Configurá tu identidad y dejá constancia en el archivo decisiones.md de cómo lo hiciste.

-Pasos que realice para configurar y preparar mi repositorio:

Primero entre al repositorio asignado por el profesor
entre a mi terminal y con el comando cd me corri hasta la carpeta creada por mi para la materia Ingenieria de Software III

Una vez que entre a esa carpeta puse en mi terminal 
git clone y la URL del repositorio dado por el profesor

Me aparecio en la terminal que realice con exito el clonar el repositorio.
 
-Configurá tu identidad y dejá constancia en el archivo decisiones.md de cómo lo hiciste.

Para realizar la configuracion de la identidad lo primero que realice fue moverme en la terminal a mi carpeta clonada del git y corri los siguientes comandos:

 git config user.name "Sofia Tula"
 git config user.email "2320454@ucc.edu.ar"


2. Desarrollar una funcionalidad
Trabajá en una rama separada de main.
Hacé al menos 2 commits atómicos con mensajes claros.
Justificá la estrategia que usaste (¿por qué esa rama? ¿por qué esos commits?).

El paso que realice aca fue crear una rama en el git desde mi terminal con el siguiente paso:
git branch sofi
Y para poder moverme a mi branch fue con el siguiente paso:
git checkout sofi

Lo proximo que realice fue: escribir una funcion de suma en visual studio code en la carpeta app.js y subir mi codigo por medio de la terminal con los siguientes comandos:

-cd src (el nombre de mi carpeta) para poder moverme 
-git status 
-git add .
-git commit -m "Mensaje"
-git push (para poder subir lo realizado a git)

Ahora lo que realice fue otra funcion pero de restar
y realice los mismos pasos nombrados anteriormente.

Estrategia:
Cree una rama separada de main para trabajar en la nueva funcionalidad.
Esto permite:

Mantener la rama main siempre estable y libre de cambios experimentales.
Desarrollar y probar la funcionalidad sin afectar el código principal.
Facilitar la revisión y fusión de cambios cuando estén listos.


3. Corregir un error (simulado) y aplicar el fix
Simulá un error en main y resolvelo en una rama hotfix.

Primero lo que realice fue crear una nueva rama que se llame hotfix.
Despues me movi nuevamente a main en la terminal con el comando:
 git checkout main
 
Estando en la rama Main, cree una funcion de sumar y forje un error de codigo, lo guarde y lo subi al repositorio con los siguientes pasos:

-Git status 
-Git Add .
-Git commit -m "Mensaje"
-Git push 

y aparecio sin problemas la funcion y el mensaje en la rama Main.

Para resolver un error de la rama Main pero en la rama hotfix realice los siguientes pasos:

Primero me movi a mi rama hotfix,luego estando en la rama hotfix realice el siguiente comando 
Git merge Main , esto lo realice para poder traer la informacion que tenia en el main y poder solucionarlo en la rama hotfix como fue pedido.

luego realice
-Git status 
-Git Add .
-Git commit -m "Solucione el problema de codigo en la funcion"
-Git push

Y aparece bien en la rama Hotfix el mensaje 

Aplicá el fix a main y también a tu rama de desarrollo.

Para hacer este paso realice lo siguiente:
Me movi a mi rama main y realice un git merge hotfix 
de esa manera me aparecio sin problemas la funcion dado que el problema fue solucionado en la rama hotfix.

Realice lo mismo en la rama sofi pero me di cuenta que no habia forjado un error en esa rama , pero si lo hubiese tenido, hubiese realizado los mismos pasos que realice con anterioridad para resolver el problema en la rama hotfix y hacer el git merge en la rama sofi para poder tener toda la funcion solucionada.

4. Hace un PR y aceptalo
Para hacer el Pull Request voy a GitHub a mi repositorio y voy a mi branch Sofi.
	- Luego voy a pull request y toco en New Pull request.
	- Tengo que poner como base el main y compare sofi, y creo el pull request.
	- Como me permitio realizar el request, me voy ahora a mi branch main.
	- Voy para pull request y me va aparecer el request que hice anteriormente.
	- Acepto el pull request.

5. Crear una versión etiquetada
Marcá una versión estable con el tag v1.0.
Explicá en decisiones.md qué convenciones usaste y por qué.

Aca lo que realice fueron los suguientes pasos: 
Me movi a mi rama main con: 
git checkout main 
Una vez en mi rama realice lo siguiente:
git tag -a v1.0 -m "v1.0: Primera version estable" 
git push origin v1.0

la version estable va a ser mi main 
Esto lo que permita es que sea facil identificar y entender. 





