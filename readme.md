*-¿Qué comandos utilizaste en el paso 11? ¿Por qué?*
git reset --hard HEAD~1
Para volver al commit anterior al actual y borrar el trabajo que tuviera en el working copy

*-¿Qué comandos utilizaste en el paso 12? ¿Por qué?*
git reflog => Para conocer el hash del commit al que quiero volver

git reset --hard 3bad430 => Para volver al commit previamente descartado

*- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?*
Ningún conflicto, styled ya contenía el trabajo de master

*- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*
Si, hemos modificado las mismas lineas en ambos archivos y eso es motivo de conflicto(siempre)

*- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?*
No genera conflicto, porque es un merge fast forward que solo implica avanzar master a styled

*- ¿Qué comando o comandos utilizaste en el paso 25?*
git log --graph

*- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?*
Si podría, porque el branch de title contenía todo el trabajo común de master.

*- ¿Qué comando o comandos utilizaste en el paso 27?*
git reset HEAD~1

*- ¿Qué comando o comandos utilizaste en el paso 28?*
git stash

*- ¿Qué comando o comandos utilizaste en el paso 29?*
git branch -D title

*- ¿Qué comando o comandos utilizaste en el paso 30?*
git reflog
git reset HEAD~2
git checkout -b title
git add git-nuestro.md
git commit -m "Titulo de nuevo"
git checkout master
git merge title

*- ¿Qué comando o comandos usaste en el paso 32?*
git reset ec40f7a
*- ¿Qué comando o comandos usaste en el punto 33?*
git reset 1a29ee3
