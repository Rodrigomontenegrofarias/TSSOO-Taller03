# TSSOO - taller03

Rodrigo Montenegro Farias - <rodrigo.montenegro@alumnos.uv.cl>

>`Universidad de Valparaíso`

# Introducción
El presente trabajo esta compuesto por un codigo en c++, y su informe, su objetico es implementar paralelismo con OpenMP.
Una vez analizado el proceso de diseño presentado en el informe mencionado, se trabajó a través del lenguaje de programación c++, con el cual manejaremos threads para cumplir con el objetivo del taller. Es importante destacar que el objetivo de este taller es implementar un programa que llene un arreglo de números enteros y luego sume los datos. Cada tarea se debe realizar de forma paralela, implementadas con OpenMP.

Además se agregó el código del taller02,  el cual se solicito la creación de hilos para cumplir una tarea similar, La funcion del codigo es incluir parametros, solo para comparar los tiempos de ejecución y llegar a una conclusión luego de analizar los tiempos.

Los parametros para ejecutar nuestro codigo son
> ./ sumArray -N  -t   -l   -L  [-h]
>
>Parámetros:
>
>-N : Numero de tamaño del arreglo.
>
>-t : Número de hilos ocupados.
>
>-l : Numero limite inferior, de rango aleatorio.
>
>-L : Numero límite superior, rango aleatorio.
>
>[-h] : muestra la ayuda de uso y termina. 
>


# Solución:

La solución del problema planteada parte con separación de dos módulos que contienen los parámetros asociados al ejecutar nuestros archivo, el primer modulo seria de llenar el arreglo, el segundo de sumar el contenido, se agregó un gráfico que demuestra comparaciones en función del tiempo total de nuestra secuencias tanto serial como paralela, además de nuestra rapidez y eficiencia.

# Primer módulo:


En el módulo uno, se implementó un arreglo cuya funcionalidad es almacenar los datos aleatorios, para luego a través de OpenMP, almacenarlos de manera paralela con una cantidad  de hilos. La API se encarga de paralelizar el código, el cual llena el arreglo base con los datos aleatorios.

# Segundo módulo:

En este segundo módulo se ocupó directamente de forma paralela la API OpenMP para sumar los valores aleatorios almacenados en el arreglo.


# Conclusión:
Para finalizar luego de implementar este programa mediante cada módulo, funcionamiento paralelo y serial, podemos realizar pruebas en base a desempeños de tiempo, rapidez, eficiencia.
Luego de visualizar y analizar cada desempeño, nos damos cuenta que existen herramientas de programación que hacen los procesos mucho más rápido, en este caso un API de OpenMP, el cual fue difícil conocer los términos necesarios pero nos permite ahorrar código y ganar tiempo de eficiencia en nuestro caso.


