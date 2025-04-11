# Preguntas

## 1) ¿Cómo te ha ayudado Git a mantener un historial claro y organizado de tus cambios?
Me ayudo a tener un entorno de trabajo más organizado ya que puedo trabajar en distintas ramas y realizando ciertas acciones sin perder versiones anteriores. Por lo cual me servira a largo plazo cuando trabaje con proyectos 
a gran escala.
## 2) ¿Qué beneficios ves en el uso de ramas para desarrollar nuevas características o corregir errores?
Al trabajar en distintas ramas permitira a otros colaboradores trabajar un codigo en paralelo , sin alterar este y manteniendo versiones anteriores.
## 3) Realiza una revisión final del historial de commits para asegurarte de que todos los cambios se han registrado correctamente.
Mediante el comando *git log --oneline* visualiza especificamente los commits junto al mensaje proporcionado.
<p align="center">
  <img src="https://github.com/user-attachments/assets/a9f91176-11aa-4370-82d1-2797dc94b796" alt="ejercicio01" width="500">
</p>

## 4) Revisa el uso de ramas y merges para ver cómo Git maneja múltiples líneas de desarrollo.
Con el uso del comando *git log --graph* logro verificar los commits y sus respectivas ramas creadas. 
<p align="center">
  <img src="https://github.com/user-attachments/assets/d6e499ad-77f0-487b-a90d-f803fad5fdf9" alt="ejercicio01" width="500">
</p>
Para el caso de merges , utilizamos el comando *git checkout "nombre-rama"* primero vamos a la rama en que deseamos fusionar y luego fusiona la rama de características con el comando
*git merge feature/"nombre-rama"*.
<p align="center">
  <img src="https://github.com/user-attachments/assets/09c0d5ed-0708-4d34-a27a-3cf30dc84d75" alt="ejercicio01" width="500">
</p>

De paso elimino la rama anterior después de fusionarla.

# Ejercicio 01
Creamos la rama feature/advanced-feature y nos conectamos a ella , editamos main.py , lo añadimos y realizamos el commit.
<p align="center">
  <img src="https://github.com/user-attachments/assets/b7056ca6-a41b-4b6f-8556-5400a188b85d" alt="ejercicio01" width="500">
</p>
Cambiamos a la rama master
<p align="center">
  <img src="https://github.com/user-attachments/assets/2f6ca416-820c-421e-aec2-8c7d02a574c3" alt="ejercici01-2" width="500">
</p>
Realizamos el merge con la rama feature/advanced-feature , resolvemos el conflicto manualmente abriendo el archivo main.py . Luego , añadimos el archivo y realizamos el commit , por ultimo eliminamos la rama feature/advanced-feature.
<p align="center">
  <img src="https://github.com/user-attachments/assets/6f7f0cd4-fc96-4e60-8c04-416ab00b32f0" alt="ejercici01-2" width="500">
</p>

# Ejercicio 02
Exploramos la historia de los commits
<p align="center">
  <img src="https://github.com/user-attachments/assets/e912f3a1-427f-4448-ba25-eb7c6b98696c" alt="ejercici01-2" width="400">
</p>
Revisamos los commits realizados por nuestro usuario
<p align="center">
  <img src="https://github.com/user-attachments/assets/b76e4423-41c0-479f-a2ac-fb7dc6b5d5bc" alt="ejercici01-2" width="400">
</p>
Hago un git revert especificamente en uno de mis commits , agregando su hash y verificamos en el historial
<p align="center">
  <img src="https://github.com/user-attachments/assets/39e5651d-0a95-4b76-a0c0-9f38973a1781" alt="ejercici01-2" width="400">
</p>
Realizo un git rebase
<p align="center">
  <img src="https://github.com/user-attachments/assets/0f60a5d3-6355-4b8a-947d-8986a8bc4dc4" alt="ejercici01-2" width="400">
</p>
Combino los 3 commits , utilizando squash en el editor que se abre.
<p align="center">
  <img src="https://github.com/user-attachments/assets/eb235f38-a37f-402f-9af0-a0c6c18e5620" alt="ejercici01-2" width="400">
</p>
Visualizamos el historial de commits
<p align="center">
  <img src="https://github.com/user-attachments/assets/cb2661c9-33bb-4827-8560-376daa74f71f" alt="ejercici01-2" width="400">
</p>

# Ejercicio 03
Vemos el historial de commits , creamos una nueva rama y nos conectamos a ella , realizamos modificaciones en el archivo main.py , lo añadimos y realizamos el commit.
<p align="center">
  <img src="https://github.com/user-attachments/assets/49ed58b8-dd76-42bf-83b9-cf905935314f" width="500">
</p>
Nos conectamos a la rama master , realizamos el merge y por último eliminamos la rama bugfix/rollback-feature
<p align="center">
  <img src="https://github.com/user-attachments/assets/20c93ef3-757f-4fec-b3ab-b5ef4de8a60e" width="500">
</p>

# Ejercicio 04
Modificamos el archivo main.py , lo agregamos y realizamos el commit 
<p align="center">
  <img src="https://github.com/user-attachments/assets/07221ba3-1a79-41fc-b369-d64479265623" width="500">
</p>
Deshacemos el commit y realizamos un cambio en README.md y luego usamos git restore para deshacer ese cambio
<p align="center">
  <img src="https://github.com/user-attachments/assets/d21a3f3f-9ff9-40b3-8560-080a3c868186" width="500">
</p>

# Ejercicio 05 
Realizamos el git clone y creamos la rama feature/team-feature
<p align="center">
  <img src="https://github.com/user-attachments/assets/b5b141b7-d83a-4804-99c5-121945153e1d" width="500">
</p>
Realizamos cambios en los archivos
<p align="center">
  <img src="https://github.com/user-attachments/assets/03b02bd4-4590-4ee0-a7df-2593bd1860a8" width="500">
</p>
Agregamos y realizamos el commit
<p align="center">
  <img src="https://github.com/user-attachments/assets/cec4d8e0-33b6-4066-bdae-f1a1e501d7b1" width="500">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/6f1f0292-0616-417b-a760-3df23a881384" width="500">
</p>
Enviamos la rama al repositorio que tenemos
<p align="center">
  <img src="https://github.com/user-attachments/assets/a464ac8f-1bb2-40f7-adb2-ba0671fed4d6" width="500">
</p>
Realizamos un pullrequest entre  feature/team-feature y nuestra rama master , por último eliminamos la rama feature/team-feature y realizamos un push nuevamente. Vemos al final que pullrequest se ha eliminado.
<p align="center">
  <img src="https://github.com/user-attachments/assets/6ed8a338-d22b-4edd-94f6-56ca90cfd2f6" width="650">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/2c017c8c-d606-4672-96a2-10ce177672d1" width="500">
</p>

# Ejercicio 06
Realizamos y confirmamos cambios en main.py en la rama master.
<p align="center">
  <img src="https://github.com/user-attachments/assets/da88dd85-29e0-43cb-b665-251f272e5801" width="500">
</p>
Cambiamos a la nueva rama creada (feature/cherry-pick)
<p align="center">
  <img src="https://github.com/user-attachments/assets/447bd6ae-7f0d-49f6-8b95-19f3390bce2f" width="500">
</p>
Aplicamos el commit específico y realizamos algunos cambios en main.py pero no lo confirmamos para guardarlo temporalmente con git stash
<p align="center">
  <img src="https://github.com/user-attachments/assets/996486e5-f329-48da-af67-59dd7993f8ab" width="500">
</p>
Como presento problemas , vuelvo a repetir los pasos.
<p align="center">
  <img src="https://github.com/user-attachments/assets/d7598bdc-648a-4468-b36a-4b46dcb5cba6" width="500">
</p>
Realizamos algunos cambios y seguidamente aplicamos git stash poop.
<p align="center">
  <img src="https://github.com/user-attachments/assets/4d945901-584b-4bf9-adfc-0d42fcc68b42" width="500">
</p>
Con el git log revisamos el historial de commits y verificamos que todos los cambios se han aplicado correctamente.















