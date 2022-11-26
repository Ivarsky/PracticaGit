#¿Qué comando utilizaste en el paso 11? ¿Por qué?
	Utilicé el comando git reset --hard HEAD~1, por que necesitaba que el working copy se modificara también

# ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	git reflog para buscar el hash del commit que había perdido al hacer el hard reset,
	git reset ¨commit hash¨ para mover el head a ese commit (podría haber usado checkout),
	git restore para copiar el estado de ese commit al working copy
	
# El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
	No hubo ningún conflicto por que los commits del main ya están incluidos en styled,
	styled es una rama de main, como main no ha seguido haciendo mas commits desde que styled se bifurcó todos sus commits están ya en styled

# El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
	Sí hubo conflictos, las líneas de texto en git nuestro son distintas

# El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
	No hubo conflicto, todos los commits de main ya estaban en styled

# ¿Qué comando o comandos utilizaste en el paso 25?
	git lg --graph

# El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
	si, la rama main no siguió haciendo commits después de la bifurcación asi que simplemente se movió al último commit de title

# ¿Qué comando o comandos utilizaste en el paso 27?
	git reset HEAD~1

# ¿Qué comando o comandos utilizaste en el paso 28?
	git add git-nuestro.md

# ¿Qué comando o comandos utilizaste en el paso 29?
	git branch -D, con -d no dejaba eliminar por que no todos los commits estaban mergeados

# ¿Qué comando o comandos utilizaste en el paso 30?
	git reflog y buscar el hash del commit del merge
	git reset hash

# ¿Qué comando o comandos usaste en el paso 32?
	git reset hash del primer commit
	
# ¿Qué comando o comandos usaste en el punto 33?
	git reset hash del ultimo commit
