# <div align="center"> Diferenciación numérica con MATLAB </div>
Este programa permite encontrar el mejor método de diferenciación numérica utilizando MATLAB.

## Tabla de contenidos
- [Objetivo del proyecto](https://github.com/luciarenata/proyecto1-com#objetivo-del-proyecto)
- [Tecnologías usadas](https://github.com/luciarenata/proyecto1-com#tecnolog%C3%ADas-usadas)
- [Problemática a resolver](https://github.com/luciarenata/proyecto1-com#problem%C3%A1tica-a-resolver)
- [Métodos de diferenciación numérica utilizados](https://github.com/luciarenata/proyecto1-com#m%C3%A9todos-de-diferenciaci%C3%B3n-num%C3%A9rica-utilizados)
- [Método](https://github.com/luciarenata/proyecto1-com#m%C3%A9todo)
- [Uso](https://github.com/luciarenata/proyecto1-com#uso)
- [Conclusiones](https://github.com/luciarenata/proyecto1-com#conclusiones)


## Objetivo del proyecto
El proyecto consiste en tomar doce métodos de diferenciación numérica, programarlos en el lenguaje de programación MATLAB y encontrar el que mejor calcula la derivada de una función dada. Este documento explica cómo lo hicimos, para qué funciona y qué concluimos. Hicimos este proyecto en febrero de 2022 para la clase de Algoritmos Numéricos por Computadora del Instituto Tecnológico Autónomo de México. Esta clase resuelve problemas matemáticos con herramientas de computación. 

## Tecnologías usadas
- Matlab Online — permite colaboración y distribución del proyecto a través de cualquier ordenador y explorador siempre y cuando se cuente con una licencia de Mathworks
- MATLAB

## Problemática a resolver
Los métodos de diferenciación son maneras de calcular la derivada de una función. No son tan exactos ni precisos como otros métodos pero se siguen usando en campos matemáticos (e.g. la resolución de ecuaciones diferenciales). Hay diferentes métodos así como diferentes maneras de calcularlos. Sus resultados son aproximaciones del valor real de la derivada de la función dada ya que son cocientes y las diferencias entre los numeradores y denominadores suelen resultar en inestabilidad. Usamos este proyecto para encontrar el método de diferenciación numérica más exacto.

## Métodos de diferenciación numérica utilizados
Los tres métodos de diferenciación numérica más comunes son los de diferenciación hacia atrás, diferenciación hacia adelante y diferenciación centrada, llamados así por los valores iniciales que toman. Las primeras y segundas derivadas hacia adelante, centradas y hacia atrás se pueden calcular usando diferencias finitas o usando coeficientes. En este proyecto calculamos cuatro funciones por método; como teníamos tres métodos (hacia adelante, hacia atrás y centrada), dos maneras de calcularlos (diferencias finitas y coeficientes) y dos grados de derivadas (primera y segunda derivada), acabamos utilizando doce funciones en total.

<p align="center">
  <img width="800" src="https://github.com/luciarenata/proyecto1-com/blob/main/diagrama.png" alt="Diagrama que enseña los tres métodos de diferenciación numérica, las dos formas de calcularlos, y las derivadas que permiten calcular.">
</p>


La Imagen 1 muestra las fórmulas que utilizamos para calcular, usando diferencias finitas, las primeras derivadas hacia delante, centrales y hacia atrás.

<p align="center">
  <img width="500" src="https://github.com/luciarenata/proyecto1-com/blob/main/formulasDFPD.png" alt="Fórmulas de las primeras derivadas usando el método de diferencias finitas.">
</p>
<p align="center"><sub> Imagen 1 </sub></p>

Las doce fórmulas son cocientes que tienen a “h” como denominador. 


## Método

Tomamos las fórmulas de diferenciación numérica y las programamos en el lenguaje MATLAB. Revisamos que fueran correctas utilizando la función de derivación de Matlab llamada “diff” y comparándola con nuestro resultado, calculando el error de la función a partir de la diferencia entre ambas cifras. 
Para poder ver la precisión de cada método, fuimos disminuyendo el valor de “h”. Hicimos once ciclos en donde achicábamos “h” por un valor de 10<sup>-1</sup> por ciclo. Esto muestra cómo existe un valor óptimo de H para cada fórmula, lo que permite reducir el error de cada método a un mínimo. Desplegamos este error en una pequeña tabla y lo graficamos en escala logarítmica para ver su variación a medida que “h” se hacía más pequeño. 

<p align="center">
  <img width="800" src="https://github.com/luciarenata/proyecto1-com/blob/main/image.png" alt="Gráfica usando los 3 métodos diferentes">
</p>
<p align="center"><sub> Gráfica 1 </sub></p>


## Uso
1. Descarga el archivo [conclusioneslivescript.mlx](https://github.com/luciarenata/proyecto1-com/blob/main/conclusioneslivescript.mlx) de este repositorio. 

2. Entra a la página de [Mathworks](https://la.mathworks.com/products/matlab-online.html?requestedDomain=) para poder utilizar Matlab Online.

3. Haz clic derecho en “Empiece a utilizar MATLAB ONLINE”.
<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/5sdlrIhrJrUYZfLchqte3RpCbIRW0pqJOeEJrsWx3i-QlcDCPEUes8GyIM5kk8jyx0_xXSjLcbg6BzxfPLQv_GUA26vATdG2MY6FdmkIdnJrqf3W1pFYguk1pC4igd020yvPilWT" alt="Página de inicio de Matlab Online.">
</p>
<p align="center"><sub> Imagen 2 </sub></p>

4. A continuación se te pedirá ingresar tus datos de acceso para Matlab. En caso de que no cuentes con una cuenta de Matlab, deberás crear una. (Es indispensable que cuentes con una licencia de Mathworks).

5. Descarga el archivo .mlx del proyecto en su ordenador.

6. Sube el archivo .mlx en [Matlab Drive](https://drive.matlab.com/files/). Esto se puede hacer a través de un ‘Drag and Drop’ o, alternativamente, utilizando la opción de “Upload” en la parte superior izquierda. 
<p align="center">
  <img width="800" src="https://lh5.googleusercontent.com/u9dSL-YBnkxW9DTOFOlPtiR0lZF7Iuz9tYVqYSno5aEVwiMiLooyPEH_r1pS7kCsTmEeFhThStDvx0etDF2MWOEaM_jzDriWT-2v95_jVbnZStPs9aEOE-08GHuDPDPs2a2UWUF6" alt="">
</p>
<p align="center"><sub> Imagen 3 </sub></p>

7. Regresa a Matlab Online y refresca la página. El proyecto ahora deberá aparecer en la barra izquierda. Haz doble clic derecho sobre el proyecto para abrirlo.

<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/8jaZAUeQ_02lwLQJRBnbkUVohZY1ZGWmJ4fdTYtkcABnX1e5qqWBb9xs74DdHkoZ5laLwh9BisJZF2GmnIIwHwEMG9bTv62FEob2gOhi0LrrdDLIDy3Fj-88HriLi1gorOPbAAQP" alt="">
</p>
<p align="center"><sub> Imagen 4 </sub></p>

8. Para correr el programa, haz clic derecho en el botón de “Run” en la barra superior.
<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/y_rRE_vC_tGJpEFXbvveyyztUL1N83jzpzCyhCCxvhDyxbLqaN2VAdayzY3lD2ajUv4QPgvXaKkSfK68jZ_leAUb2fh5gM3xPaBlJB1-_x7JmhjNjYNfKib0KAKLSv6S95PGRidw" alt="">
</p>
<p align="center"><sub> Imagen 5 </sub></p>

9. Se abrirá una pestaña a la derecha con los resultados del LiveScript. Aquí podrás navegar los resultados y las gráficas de las pruebas realizadas.
<p align="center">
  <img width="800" src="https://lh6.googleusercontent.com/higQHv01eDa0ZGapSvNGqkm1XNjNNAFdXy6UgI4zl-Mbh97oOgRK3o2wi7EFI3tXaBxxnaCNDqRqCD9lXTuWPSxmQt4T1UYViIgnyuiEpS6U2UV751H8j1TGofMtUrxGD9R_z1cS" alt="">
</p>
<p align="center"><sub> Imagen 6 </sub></p>

## Conclusiones
Este proyecto permite ver que el método óptimo de diferenciación numérica es el de diferencias centradas usando coeficientes tanto para la primera como para la segunda derivada. Es el que menor error presenta. 
