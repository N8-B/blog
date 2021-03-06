### 5 comandos imprescindibles para el día a día con [GIT](https://git-scm.com/)
Pocas veces utilizamos todo el potencial de GIT mayormente
porque desconocemos todas sus funcionalidades o lamentablemente
por pereza. Hasta que llega ese día en que
hacemos `$ git push` apurado y..  

![git push gif](http://i.imgur.com/sFmkFjT.gif)	

Oh Dios.. *n* errores han aparecido, el mensaje del commit es incorrecto, has subido más cambios de lo deseado.. ¿ Y ahora ? ¡Ayúdame Google!    
Estos son **5** comnandos sencillos para evitar llegar a este punto:
 - `$ git commit --amend` Nos permite modificar el mensaje del último commit realizado, siempre que no hayamos echo un *push* a origen con él
 - `$ git stash [comando]`   
    El [stash](https://git-scm.com/docs/git-stash)  de GIT permite guardar todas las modificaciones en el entorno de trabajo actual y dejar limpio nuestro entorno de trabajo, o sea listo para cambiar de rama, hacer un commit, algún cambio de última hora sin interferir el trabajo actual o mergear con otra rama.     
    La manera más común de usar la pila es hacer cambios en una rama y ejecutar `$ git stash save` para salvar las modificaciones en el entorno actual, en este momento no vemos ningún cambio en nuestra rama, mergeamos o comiteamos algún cambio y seguidamente podemos retornar los cambios en los que estábamos trabajando con `$ git stash pop`. Usamos `$ git stash list` para ver todas las salvas en la pila.
 - `$ git add -p [archivo]`     
    Nos permite añadir y validar por archivo bloque a bloque los cambios que queremos añadir al commit.     
Digamos que hemos echo varias modificaciones y solo queremos subir la modificacion *x*, pues con el flag `-p` esto es posible ya que podremos seleccionar cuales de las modificaciones queremos añadir y cuales no.
 - `git log | grep "texto" -m 10 -A 5`      
    Este es uno de mis preferidos, con la unión de dos comandos [git log](https://git-scm.com/docs/git-log) y [grep](http://www.gnu.org/software/grep/manual/grep.html#Introduction) podemos listar en el terminal los commits que contengan "texto" en su mensaje de commit. Por defecto git log muestra un histórico ordenado de commits con sus mensajes, grep lo utilizamos para filtrar de estos solo los que nos interesan.      
 - `$ git push origin <branch>` 
    Es muy fácil haber echo varios commits en local en varias ramas, por lo que es importante cuando vamos a hacer un `push` solo subir los cambios de la rama que queremos, así que añadimos los parámetros `origin <Nombre de la rama>` para garantizar que solo se suban los cambios de la rama que queremos.      

### Bonus
 - **Commits sobre pequeños cambios**: todo comienza con realizar los commits lo más atómico posible, con esto garantizamos una mejor trazabilidad de los cambios y la suficiente independencia entre estos que nos permita movernos de un commit a otro sin dañar toda la estabilidad de la feature.

Para terminar es recomendable siempre hacer los commits con `$ git commit` para escribir un mensaje correcto y asegurarnos de que solo vamos a subir las modificaciones que queremos.
