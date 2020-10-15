# PCPractica4
En ésta práctica se hace uso de el método de variable de cerradura,
el cual utiliza una variable compartida llamada cerradura. ´
Si se desea que un proceso entre a su SC, primero se hace una prueba de cerradura, es decir,
se pregunta por el valor de la variable cerradura, si es cero, entonces el proceso cambia el
valor de la variable a uno y entra a su SC. en caso contrario, el proceso espera por un tiempo
ddeterminado por el S.O., entonces el proceso espera hasta obtener el valor cero de nuevo.

Éste método NO cumple con las 4 condiciones de Exclusión mutua
El problema de este metodo consiste en que el proceso que está en su S.C. no avisa cuando ´
deja esta, provocando así que los demas procesos no se enteren del momento que el recurso
compartido este disponible, es decir, que los demas procesos no saben cuando la cerradura es ´
cero
