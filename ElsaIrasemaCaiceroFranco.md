1. ¿Qué es un sistema de control de versiones?
(VCS) Version Control System es una metodología o herramienta  que nos ayuda a dar un seguimiento de cambios que hacemos en nuestros archivos del proyecto. 
	
1. ¿Cuáles son los objetivos de un sistema de control de versiones?
Mantener y proveer acceso a cada versión que un archivo ha tenido desde que se almacenó y proveer un forma de metadatos

1. ¿Cuáles son las pautas para controlar los cambios de diseño?
Damos seguimiento  a los cambios gracias a las herramientas de VCS que mantiene una copia de cada cambio realizado.

Seguir un procedimiento sistemático de control de cambios
• Manejar solicitudes de cambio en grupos
• Estimar el costo de cada cambio
• Tener cuidado con los grandes volúmenes de cambio
• Establecer un tablero de control de cambios o su equivalente de una manera 
que tenga sentido para el proyecto
• Esté atento a la burocracia, pero no permitir que el miedo a la burocracia 
impida un cambio efectivo
 
1. ¿Qué es un repositorio?
Es un lugar donde el sistema de control de versiones mantiene el seguimiento de todos los cambios realizados. 

1. ¿Qué se debe almacenar en un repositorio?
Todo. Todo lo que tenga que ver con nuestro proyecto y obviamente, el código fuente, su archivo de compilación (makefile, build.xml), de configuración y pruebas de unidad

1. ¿Cómo se puede determinar que incluir en un repositorio?
La clave es preguntarse a sí mismo "Si no tengo X, ¿podría yo trabajar en este proyecto? ". 
Si la respuesta es no podría, entonces deberías incluirlo en el repositorio. 

1. ¿Qué es un *Working Tree*?
Es la vista actual dentro del repositorio. Es donde hacemos nuestros cambios.  Allí están los archivos de nuestro proyecto: el código fuente, archivos de compilación, pruebas unitarias, etc. 
En algunos VCS le llaman "working copy" y se puede separar el "working tree" del repositorio. 

La vista actual del flujo de cambios y o modificaciones de rchivos dentro de nuestro proyecto

1. ¿Qué hace un *commit*?
Agrega una nueva versión al repositorio y almacena el mensaje de log y explica el cambio que hizo

1. ¿Qué ocurre cuando se hace *push*?
Se utiliza para subir confirmaciones de cambios realizdas en un rama local a un repositorio remoto

1. ¿Qué ocurre cuando se hace *fetch*?
Contrario al push. Obtiene los cambios de un repositorio remoto.

1. ¿Qué es un *branch* o rama?
Una rama es una "versión" distinta  que tiene una historia diferente a las demás.

Es el seguimiento de los cambios en su contenido separado por otras ramas para que se puedan crear versiones alternativas. Se ocupan para desarrollar funcionalidades aisladas.

1. ¿Qué es un *merge*?
Es la unión de dos o más ramas combinando sus historias en una. El repositorio trata de comparr dos archivos y determinar los cambios. En algunos casos si los cambios se dieron en líneas diferentes hace el merge automáticamente. Si hay cambios en la misma línea sucede un conflicto.

Proceso de combinar dos ramas, estos cambios deben ser aprobados por los colaboradores.

1. ¿Qué es un *strict locking*?
Restringe que un archivo pueda ser modificado al mismo tiempo por dos personas diferentes hasta 
Si alguien quiere modificar x archivo y este está siendo editado por otro integrante, entonces no podrá modificarlo mientras esté editándolo alguien más.
Se pide al repositorio para hacer cambios a  1 artefacto y evintando cambios simultáneos.

1. ¿Qué es un *optimistic locking*?
Permite que múltiples desarrolladores trabajen en el mismo código en el mismo archivo con la suposición de que la mayoría de estos archivos no tendrán conflicto. 

