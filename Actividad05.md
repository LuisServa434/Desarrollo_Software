# Actividad 05
## 1) Fusión Fast-forward (git merge --ff)
Creamos un nuevo repositorio y realizamos la conexión con el comando `git.init`
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 003838.png" alt="ff-parte01" width="600">
</p>

Agregamos el archivo `README.md` en la rama main , lo agregamos y realizamos el commit.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 003858.png" alt="ff-parte01" width="600">
</p>

Creamos la nueva rama y nos conectamos a ella , modificamos el archivo README.md y realizamos un commit en la nueva rama. Por úlltimo regresamos a la rama main y realizamos el comando `git.merge` , se logro ya que durante el trabajo con la rama add-description no hubo ningun otro commit en la rama principal.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 003906.png" alt="ff-parte01" width="600">
</p>

## 2) Fusión No-fast-forward (git merge --no-ff)
Creamos un nuevo repositorio y realizamos la conexión con el comando `git.init`.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004226.png" alt="ff-parte01" width="600">
</p>

Agregamos un archivo con contenido `README.md` en la rama main y luego realizamos su commit. Por último creamos y nos conectamos a la nueva rama llamada add-feature.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004236.png" alt="ff-parte01" width="600">
</p>

Desde la nueva rama , añadimos contenido al archivo `README.md` , realizamos el commit y nos conectamos a la rama main para realizar la fusión mediante el comando `git merge --no-ff`. Por último vemos una representación de la fusión con el historial de los commits.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004246.png" alt="ff-parte01" width="600">
</p>

## 3) Fusión squash (git merge --squash)
Creamos el nuveo repositorio y nos conectamos con el comando `git.init`.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004819.png" alt="ff-parte01" width="600">
</p>

Creamos el archivo `README.md` y añadimos contenido , realizamos el commit en la rama main y luego creamos y nos conectamos a la rama add-basic-files.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004832.png" alt="ff-parte01" width="600">
</p>

Añadimos contenido al archivo `CONTRIBUTING.md` y `LICENSE.txt` , realizamos los commits para cada archivo.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004841.png" alt="ff-parte01" width="600">
</p>

Nos conectamos a la rama main para hacer la fusión y ralizamos el commit que fusionara todo en uno solo.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 004854.png" alt="ff-parte01" width="600">
</p>

## Resolver conflictos en una fusión non-fast-forward
Creamos el repositorio y creamos el .git .
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 010607.png" alt="ff-parte01" width="600">
</p>

Creamos el archivo `index.html` y realizamos un commit desde la rama main. Por último , creamos y nos conectamos a la rama feature-update.  
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 010617.png" alt="ff-parte01" width="600">
</p>

Desde la nueva rama editamos el archivo `index.html` , realizamos el commit y nos conectamos a la rama main. y modificamos el archivo `index.html` y realizamos el commit . Por último realizamos la fusión , como presenta problemas lo resolvemos manualmente y después de eso realizamos el commit y vemos que se logro fusionar.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 010634.png" alt="ff-parte01" width="600">
</p>

- ¿Qué pasos adicionales tuviste que tomar para resolver el conflicto?
  
  Configure manualmente el archivo `index.html` eliminando las lineas que ocasionan este conflicto (para esto podemos utilizar nano index.html) , luego agregue dicho archivo y realice su commit , al final nos muestra un mensaje que la fusión fue exitosa.

- ¿Qué estrategias podrías emplear para evitar conflictos en futuros desarrollos colaborativos?
  
  Este método es más recomendable para proyectos pequeños o medianos, donde el número de ramas y colaboradores es manejable. En proyectos grandes, requiere configuraciones manuales para cada fusión y esto signfica que toma más tiempo , por lo cual sería inviable. Sin embargo ,  el método de merge non-fast-forward permite mantener un historial más claro de cuándo se integran los cambios de una rama al proyecto principal.

## Comparar los historiales con git log después de diferentes fusiones
Creamos el nuevo repositorio y nos conectamos a la rama main.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 014027.png" alt="ff-parte01" width="600">
</p>

Creamos el archivo `version.txt` , realizamos el commit y luego creamos la rama feature-1 y modificamos el archivo `version.txt`.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 014044.png" alt="ff-parte01" width="600">
</p>

Creamos la rama feature-2 y modificamos `version.txt`. Luego nos conectamos a main:
- Fusionamos feature-1 usando fast forward.
- Fusionamos feature-2 sando non-fast-forward.
Por último creamos y nos conectamos a la rama feature-3 , modificamos el archivo `version.txt` dos veces.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 014058.png" alt="ff-parte01" width="600">
</p>

Nos conectamos a la rama main y realizamos la fusión por squash.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 014130.png" alt="ff-parte01" width="600">
</p>

Realizamos el commit que fusiona todo y vemos el historial de cada tipo de fusión.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 014143.png" alt="ff-parte01" width="600">
</p>

- ¿Cómo se ve el historial en cada tipo de fusión?
  
  En el caso de fast forward vemos una estructura lineal , para el caso de non fast forward ocurre lo mismo , sin embargo nos muestra un mensaje que se ha realizado un merge , mientrás tanto en el caso de squash , se muestra un commit solo en la rama principal.

  <p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 113949.png" alt="ff-parte01" width="600">
  </p>
  Graficamente según la imagen , en feature-1 , se realizo la fusión por fast-forward sin presentar problemas. Luego , en feature-2 hubo problemas , después de eso se realiza una configuración manual , se agrega el commit y la fusión logra completarse . Por último en feature-3 se muestra los commits en esa rama que luego son fusionados en uno solo en la rama main.

- ¿Qué método prefieres en diferentes escenarios y por qué?
  
  En el caso de fast-forward prefiero usarlo en un escenario donde trabajo yo solo o cuando son cambios pequeños.
  En un escenario donde el proyecto es pequeño o mediano y se debe colaborar , utilizaría non-fast-forward ya que permite visualizar las actividades en las ramas. Por último , para un escenario donde realizo varios commits en una rama , eligiria squash y de esa forma lo fusiono y reduzco todo desde una rama principal , de esa forma evito congestionar el repositorio de tantos commits.

## Usando fusiones automáticas y revertir fusiones
Creamos la carpeta y luego inicializamos .git.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020417.png" alt="ff-parte01" width="600">
</p>

Creamos el archivo `file.txt` y realizamos dos commits.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020434.png" alt="ff-parte01" width="600">
</p>

Creamos una nueva rama auto-merge y modificamos el archivo `file.txt` , para luego hacer su respectivo commit.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020450.png" alt="ff-parte01" width="600">
</p>

Regresamos a la rama main , modificamos el archivo `file.txt` y realizamos la fusión , vemos que no es posible y se presenta un problema.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020520.png" alt="ff-parte01" width="600">
</p>

Realizamos la configuración manual.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020605.png" alt="ff-parte01" width="600">
</p>

Luego de corregir el error continuamos con el merge , revertimos la fusión y luego verificamos el historial.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 020636.png" alt="ff-parte01" width="600">
</p>

- ¿Cuándo usarías un comando como git revert para deshacer una fusión?
    - Cuando la fusión ya fue subida al repositorio y no se puede usar reset sin afectar a otros.
    - Para deshacer una fusión sin borrar el historial.
    - Si la fusión causó errores o rompió el proyecto, y se quiere volver al estado anterior de forma segura.  

- ¿Qué tan útil es la función de fusión automática en Git?
    - Es muy útil porque ahorra tiempo al integrar ramas sin conflictos.
    - Git detecta y fusiona cambios automáticamente en archivos distintos.
    - Solo requiere intervención si hay conflictos entre ramas.
    - Ayuda a mantener un flujo de trabajo ágil y ordenado.

## Fusión remota en un repositorio colaborativo
Para este ejercicio tenemos que tener otra cuenta de git hub.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 021647.png" alt="ff-parte01" width="600">
</p>

- Clonamos el repositorio
- Creo la nueva rama colaboracion
- Creo el archivo `colaboracion.txt` , lo agrego y realizo el commit.
- Por último subo este archivo a mi repositorio creado desde github , se genera un enlace donde realizare el PullRequest.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 022407.png" alt="ff-parte01" width="600">
</p>

Pull Request en GitHub.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 021932.png" alt="ff-parte01" width="600">
</p>

- ¿Cómo cambia la estrategia de fusión cuando colaboras con otras personas en un repositorio remoto?
   - Se vuelve necesario mantener el repositorio actualizado con git pull frecuentemente.
   - Es mejor usar merge con commits de fusión (--no-ff) para tener claro qué cambios vienen de qué ramas.
   - Se recomienda trabajar con pull requests (PR) para revisar y discutir cambios antes de fusionarlos.    
- ¿Qué problemas comunes pueden surgir al integrar ramas remotas?
   - Conflictos de fusión, cuando dos personas modifican las mismas líneas de un archivo.
   - Historial confuso si se mezclan muchos merges sin orden o sin squash.
   - Desactualización: si alguien trabaja mucho tiempo sin hacer pull, puede tener problemas al hacer push.
   - Fusiones innecesarias o mal hechas, que pueden romper funcionalidades o duplicar código.
     
## Ejercicio final : flujo de trabajo completo
- Creo el directorio ejercicio_final y inicializo .git.
- Creo el archivo `README.md` y realizo el commit desde la rama main.
- Creo las dos ramas feature1 y feature2.
- Me conecto a la rama feature1 y modifico el archivo `README.md`.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093328.png" alt="ff-parte01" width="600">
</p>

- Realizo el commit en la rama1.
- Me conecto a la rama2 y modifico el archivo `README.md` y realizo el commit desde esa rama.
- Por último me conecto a la rama main.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093359.png" alt="ff-parte01" width="600">
</p>

- Realizo una fusion por fast-forward a la rama feature1.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093415.png" alt="ff-parte01" width="600">
</p>

- Realizo una fusion por non-fast-forward a la rama feature2 , como se presenta problemas lo resuelvo manualmente , realizo el commit y se logra la fusión.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093432.png" alt="ff-parte01" width="600">
</p>

- Creo la rama adicional feature3.
- Modifico el archivo `README.md` y realizo dos commits en dicha rama.
- Me conecto a la rama main y realizo la fusión por squash , agregando el respectivo commit que fusionara todo.
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093458.png" alt="ff-parte01" width="600">
</p>
<p align="center">
  <img src="imagenes\Captura de pantalla 2025-04-14 093505.png" alt="ff-parte01" width="600">
</p>
Verificamosor el historial de commits. En la imagen se muestra el primer commit de la rama main "Añadiendo README.md" , luego se realizo el commit de feature1 fusionandolo por fast-forward sin problemas . Segundo , se realizo la fusión con feature2 por non-fast-forward pero hubo problemas que tuvieron que modificarse manualmente y luego se logro fusionar y como resultado tenemos el mensajae de Merge que nos indica el éxito de esta fusión . Por último la fusión por squash se resume con el ultimo commit en la rama main.
