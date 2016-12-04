#¿Qué comando utilizaste en el paso 11? ¿Por qué?
>Utilizé el comando git reset --hard HEAD~1 porque con colocar el puntero en el
commit padre (HEAD~1) e indicarle que me modifique mi working copy (--hard) 
obtengo el resultado que se me indicaba.  
#¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
>Me dispuse a utilizar el mismo comando que en el paso numero 11, solo que esa vez
en vez de hacer referencia al commit padre, hice referencia a la referencia
corta del commit que realizamos para poner estilos al git-nuestro.md.
Tanto el commit que necesitaba como la referencia al mismo la obtuve usando el 
comando "git reflog"  
#El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
>No causó ningún conflicto porque el único commit de la rama master ya lo teníamos
también el la rama styled.  
#El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
>Causó conflicto porque en el archivo git nuestro teníamos versiones distintas de LAS
MISMAS lineas, entonces git no puede determinar por nosotros con cuales ha de 
quedarse.  	
#El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
>No causó conflicto porque no había distintas versiones de ninguna linea.
(Como styled absorvió a master y el conflicto entre htmlfy y styled lo resolvimos
quedandonos con lo que habia en styled resulta que en realidad el archivo era idéntico
tanto en styled como en master).  
#¿Qué comando o comandos utilizaste en el paso 25?
>Utilizé el comando "git log --graph" para poder ver los nodos dibujados en la 
consola y así "dibujar el esquema".  
#El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
>Si podría ser fastforward porque realmente solo necesitabamos avanzar el puntero
master al mismo commit que el puntero title y todos los commits anteriores eran
iguales.  
#¿Qué comando o comandos utilizaste en el paso 27?
>En ese caso utilizé el comando "git reset HEAD~1" pero desde la rama master.
Sin --hard para mantener cambios en el working copy y HEAD~1 desde master porque
para deshacer este merge solamente necesitaba dejar el commit que generó al mergear
inaccesible.  
#¿Qué comando o comandos utilizaste en el paso 28?
>Utilizé el comando "git checkout -- git-nuestro.md" y este no tiene mucha explicación
simplemente descarta los cambios en este archivo.  
#¿Qué comando o comandos utilizaste en el paso 29?
>El comando que nos solucionó este punto fué "git branch -D title" porque nos borra
la rama, tampoco es para explicar mucho aquí.    
#¿Qué comando o comandos utilizaste en el paso 30?
>Utilizé el comando "git reset --hard 9114e5a" que me situaba el puntero master 
y el puntero HEAD en el commit que creó el merge al absorver title desde master.
La dirección a este commit la saqué del reflog.
Al ubicarnos aquí, el commit vuelve a estar accesible y por tanto el merge queda
restaurado.  
#¿Qué comando o comandos usaste en el paso 32?
>Con el comando log averigué la direccion del primer commit y realizé un "git reset 
--hard" a la dirección de este.  
>¿Qué comando o comandos usaste en el punto 33?
Con el fin de no repetirme usé "git reset --hard HEAD@{1}" que me dejaba en el 
mismo punto que en el COMANDO anterior.  
