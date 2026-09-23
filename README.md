## ICC
Repositorio para la primera practica de cc
# Presentacion

Somos estudiante de la Facultad de Ciencias.

## Actualmente
- Trabajo en estudiar  todas las noches

## Preguntas Iniciales

¿Qué información almacena un commit?
Un Commit registra una version del proyecto e incluye los cambios realizados, el nombre y el correo.

¿Qué diferencia existe entre un repositorio local y un repositorio remoto?
El repositorio local guarda los cambios antes de hacer un pull mientras que el reposituorio remoto guarda todos los guardados que se han hecho

¿Qué esperan que ocurra cuando ambos integrantes modifican archivos distintos?
Pues ambos podemos modificar pero solo podremos ver los cambios que hizo el otro cuando este en el repositorio remoto

¿Qué esperan que ocurra cuando ambos modifican exactamente la misma linea?
Se sobreescribira y se guardaran ambas

## Comandos observados
nano, git push, git pull, git status, git dif. git commit
## Planeacion
Solo el Developer Bharia commit porque es el unico que va a escribir en el trabajo colaborativo.
El push lo hace el Developer B porque tiene que pasar los cambios al developer A
El pull lo hace el Developer A para que pueda ver los cambios que hizo el Developer B

## Historial esperado

D---E <-- binario
\
A---B---C <- main 
\
F---G <-- decimal

## Rechazo de git

¿Por qué Git rechazo el primer push de Developer B?
 Por no estar en la rama principal , tambien se podria decir que el devolver b no esta actualizado

 ¿Existía un conflicto de contenido?
No, por que modificamos archivos distintos
 
¿Qué ocurrió cuando ejecutaron pull?
Git descarto los cambios del remoto y los integro con los cambios locales

 ¿Qué diferencia observan entre un push rechazado y un conflicto?
 Un push rechazado no permite subir los commits, ya que le faltaba integrar cambios en el remoto, el conflicto creemos que es por que git necesita decidir cual cambio queremos.

##Pregunta

¿Realizar un merge implica necesariamente que exista un conflicto?

No. En este ejercicio Git pudo integrar automaticamente los cambios porque cada rama modifico un archivo distinto que serian decimal y binario.

## Conflicto
¿Que representa HEAD en este momento?
Donde esta o comienza el conflicto
¿Que representa el contenido entre «««< y =======?
El <<< indica donde inicia todo lo que modificamos y provoco el conflicto y el === separa la modificacion que cada uno hizo
¿Que representa el contenido entre ======= y »»»>?
El >>> indica donde terminan las modificaciones y el ===== aepara las modificaciones que cada uno hizo
¿Por que Git no pudo decidir automáticamente que contenido conservar?
Porque no habia una jerarquia de cual era mas importante para conservar# icc-practica01-git.1

## Historia real
¿En que se parece al dibujo inicial?
Solo se parecen en que las ramas salieron
 
¿En que es diferente?
En que al las ramas salian de main y regresaban y asi con todas las ramas

¿Que partes del historial no habían anticipado?
No consideramos las demas ramas de conflicto y que en merge se iban a juntar las ramas y los commits que ibamos a hacer incluyendo los que fueron por errores

¿Que entienden ahora que no entendían cuando realizaron el primer dibujo?
Que cuando integramos las ramas iban a regresar a main y que los merge provocaban eso 

## pregunta
¿Que ventaja tiene utilizar el nombre v1.0 para identificar este punto del
historial en lugar de utilizar solamente el hash del commit?

Es mas facil de recordar y reconocer, permite identificar una version mas especifica del proyecto ademas de poder encontrar el punto en el historial


