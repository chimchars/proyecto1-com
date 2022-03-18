# <div align="center"> Encontrar el mejor método de diferenciación numérica usando MATLAB </div>

## Tabla de contenidos
- [Objetivo del proyecto](https://github.com/luciarenata/proyecto1-com#objetivo-del-proyecto)
- [Tecnologías usadas](https://github.com/luciarenata/proyecto1-com#tecnolog%C3%ADas-usadas)
- [Setup](https://github.com/luciarenata/proyecto1-com#setup)
- [Problemática a resolver](https://github.com/luciarenata/proyecto1-com#problem%C3%A1tica-a-resolver)
- [Métodos de diferenciación numérica utilizados](https://github.com/luciarenata/proyecto1-com#m%C3%A9todos-de-diferenciaci%C3%B3n-num%C3%A9rica-utilizados)
- [Método](https://github.com/luciarenata/proyecto1-com#m%C3%A9todo)
- [Uso](https://github.com/luciarenata/proyecto1-com#uso)

## Objetivo del proyecto
Hicimos este proyecto en febrero de 2022 para la clase de Algoritmos Numéricos por Computadora del Instituto Tecnológico Autónomo de México. Esta clase resuelve problemas matemáticos con herramientas de computación. El proyecto consiste en tomar doce métodos de diferenciación numérica, programarlos en el lenguaje de programación MATLAB y encontrar el que mejor calcula la derivada de una función dada. Este documento explica cómo lo hicimos, para qué funciona y qué concluimos.

## Tecnologías usadas
- Matlab Online
- MATLAB

## Setup
Para facilitar la colaboración y la distribución del proyecto se utilizó Matlab Online, al cual se puede acceder desde cualquier ordenador y a través de cualquier explorador siempre y cuando se cuente con una licencia de Matlab.

## Problemática a resolver
Los métodos de diferenciación son maneras de calcular la derivada de una función. No son tan exactos ni precisos como otros métodos pero se siguen usando en campos matemáticos (e.g. la resolución de ecuaciones diferenciales). Hay diferentes métodos, todos entre ellos parecidos y con pequeñas diferencias entre sí, así como diferentes maneras de calcularlos. Sus resultados son aproximaciones del valor real de la derivada de la función dada. Usamos este proyecto para encontrar el método de diferenciación numérica más exacto.

## Métodos de diferenciación numérica utilizados
Los tres métodos de diferenciación numérica más comunes son los de diferenciación hacia atrás, diferenciación hacia adelante y diferenciación centrada, llamados así por los valores iniciales que toman. Las primeras y segundas derivadas hacia adelante, centradas y hacia atrás se pueden calcular usando diferencias finitas o usando coeficientes. En este proyecto calculamos cuatro funciones por método; como teníamos tres métodos (hacia adelante, hacia atrás y centrada), dos maneras de calcularlos (diferencias finitas y coeficientes) y dos grados de derivadas (primera y segunda derivada), acabamos utilizando doce funciones en total.

<p align="center">
  <img width="800" src="https://github.com/luciarenata/proyecto1-com/blob/main/diagrama.png" alt="Diagrama que enseña los tres métodos de diferenciación numérica, las dos formas de calcularlos, y las derivadas que permiten calcular.">
</p>
<p align="center"><sub> Diagrama 1 </sub></p>

La Imagen 1 muestra las fórmulas que utilizamos para calcular, usando diferencias finitas, las primeras derivadas hacia delante, centrales y hacia atrás.

<p align="center">
  <img width="500" src="https://github.com/luciarenata/proyecto1-com/blob/main/formulasDFPD.png" alt="Fórmulas de las primeras derivadas usando el método de diferencias finitas.">
</p>

Todas las fórmulas utilizadas son cocientes, al igual que las fórmulas de la Imagen 1. 


## Método

Tomamos las fórmulas de diferenciación numérica y las programamos en el lenguaje MATLAB. Revisamos que fueran correctas utilizando la función de derivación de Matlab llamada "diff" y comparándola con nuestro resultado, calculando el error de la función a partir de la diferencia entre ambas cifras. 
Para poder ver la presición de cada método, fuimos achicando el valor de “h”. Esto muestra cómo existe un valor óptimo de H para cada fórmula, lo que permite reducir el error de cada método a un mínimo. Desplegamos este error en una pequeña tabla y lo graficamos en escala logarítmica para ver su variación a medida que “h” se hacía más pequeño. 

<p align="center">
  <img width="800" src="https://github.com/luciarenata/proyecto1-com/blob/main/image.png" alt="Gráfica usando los 3 métodos diferentes">
</p>
<p align="center"><sub> Gráfica 1 </sub></p>

## Uso
1. Entrar a la página de [Mathworks](https://la.mathworks.com/products/matlab-online.html?requestedDomain=) para poder utilizar Matlab Online.

2.  Hacer click derecho en “Empiece a utilizar MATLAB ONLINE”.
<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/5sdlrIhrJrUYZfLchqte3RpCbIRW0pqJOeEJrsWx3i-QlcDCPEUes8GyIM5kk8jyx0_xXSjLcbg6BzxfPLQv_GUA26vATdG2MY6FdmkIdnJrqf3W1pFYguk1pC4igd020yvPilWT" alt="Página de inicio de Matlab Online.">
</p>

3.  A continuación se le pedirá ingresar sus datos de acceso para Matlab. En caso de que no cuente con una cuenta de Matlab, deberá crear una. (Es indispensable que cuente con una licencia de Matlab).

4.  Descargar el archivo .mlx del proyecto en su ordenador.

5.  Subir el archivo .mlx en [Matlab Drive.](https://drive.matlab.com/files/) Esto se puede hacer a través de un ‘Drag and Drop’ o, alternativamente, utilizando la opción de “Upload” en la parte superior izquierda. 
<p align="center">
  <img width="800" src="https://lh5.googleusercontent.com/u9dSL-YBnkxW9DTOFOlPtiR0lZF7Iuz9tYVqYSno5aEVwiMiLooyPEH_r1pS7kCsTmEeFhThStDvx0etDF2MWOEaM_jzDriWT-2v95_jVbnZStPs9aEOE-08GHuDPDPs2a2UWUF6" alt="">
</p>

6.  Regresar a Matlab Online y refrescar la página. El proyecto ahora deberá aparecer en la barra izquierda. Haga doble click derecho sobre el proyecto para abrirlo.

<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/8jaZAUeQ_02lwLQJRBnbkUVohZY1ZGWmJ4fdTYtkcABnX1e5qqWBb9xs74DdHkoZ5laLwh9BisJZF2GmnIIwHwEMG9bTv62FEob2gOhi0LrrdDLIDy3Fj-88HriLi1gorOPbAAQP" alt="">
</p>

7.  Para correr el programa, haga click derecho en el botón de “Run” en la barra superior.
<p align="center">
  <img width="800" src="https://lh3.googleusercontent.com/y_rRE_vC_tGJpEFXbvveyyztUL1N83jzpzCyhCCxvhDyxbLqaN2VAdayzY3lD2ajUv4QPgvXaKkSfK68jZ_leAUb2fh5gM3xPaBlJB1-_x7JmhjNjYNfKib0KAKLSv6S95PGRidw" alt="">
</p>

8.  Se abrirá una pestaña a la derecha con los resultados del LiveScript. Aquí podrá navegar los resultados y las gráficas de las pruebas realizadas.
<p align="center">
  <img width="800" src="https://lh6.googleusercontent.com/higQHv01eDa0ZGapSvNGqkm1XNjNNAFdXy6UgI4zl-Mbh97oOgRK3o2wi7EFI3tXaBxxnaCNDqRqCD9lXTuWPSxmQt4T1UYViIgnyuiEpS6U2UV751H8j1TGofMtUrxGD9R_z1cS" alt="">
</p>
