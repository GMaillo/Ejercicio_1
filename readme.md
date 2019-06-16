-¿Qué comando utilizaste en el paso 11? ¿Por qué?

git reset --hard HEAD~1, lo utilizamos para deshacer el último commit. Añadimos el hard para eliminar 
los cambios realizados en el working copy.

-Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

primero utilizamos git reflog para ver lo ocurrido en el repositorio, obtenemos el identificador del 
commit que creamos anteriormente y con git reset --hard (identificador) rehacemos el último commit.

-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, por que al hacer el reset con --hard eliminamos los cambios que realizamos en el working copy.

-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Sí, al crear la rama htmlify modificamos el archivo git-nuestro.md y creamos un nuevo commit. A la 
hora de hacer el merge causa conflicto por que en la modificación hemos tocado parte del anterior 
código.

-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, ya que al resolver el anterior conflicto mantuvimos el contenido de la rama styled.

-¿Qúe comando o comandos utilizaste en el paso 25?

log --graph (nos muestra el grafo), --pretty=oneline (nos muestra cada commit resumido en una línea), 
--decorate (nos muestra los punteros).

-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Sí, absorvería la información.

-¿Qué comando o comandos utilizaste en el paso 27?

Apliqué git log --graph --pretty=oneline --decorate para obtener el identificador del anterior commit 
y luego git reset (identificador) para deshacer el merge.

-¿Qué comando o comandos utilizaste en el paso 28?

gity checkout -- git-nuestro.md

-¿Qué comando o comandos utilizaste en el paso 29?

git branch -D title

-¿Qué comando o comandos utilizaste en el paso 30?

git reset (identificador commit que se creó con el merge)

-¿Qué comando o comandos utilizaste en el paso 32?

git reset (identificador commit inicial)

-¿Qué comando o comandos utilizaste en el paso 33?

git reset (identificador commit título)
