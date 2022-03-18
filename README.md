# <div align="center"> Encontrar el mejor método de diferenciación numérica usando MATLAB </div>

## Tabla de contenidos
-[Objetivo del proyecto](https://github.com/luciarenata/proyecto1-com#objetivo-del-proyecto).

-[Tecnologías usadas](https://github.com/luciarenata/proyecto1-com#tecnolog%C3%ADas-usadas).

-[Setup](https://github.com/luciarenata/proyecto1-com#setup).

-[Uso](https://github.com/luciarenata/proyecto1-com#uso).

-[Problemática a resolver](https://github.com/luciarenata/proyecto1-com#problem%C3%A1tica-a-resolver).

-[Métodos de diferenciación numérica utilizados](https://github.com/luciarenata/proyecto1-com#m%C3%A9todos-de-diferenciaci%C3%B3n-num%C3%A9rica-utilizados).

-[Método](https://github.com/luciarenata/proyecto1-com#m%C3%A9todo).

-[Conclusiones](https://github.com/luciarenata/proyecto1-com#conclusiones).

## Objetivo del proyecto
Hicimos este proyecto en febrero de 2022 para la clase de Algoritmos Numéricos por Computadora del Instituto Tecnológico Autónomo de México. Esta clase resuelve problemas matemáticos con herramientas de computación. El proyecto consiste en tomar doce métodos de diferenciación numérica, programarlos en el lenguaje de programación MATLAB y encontrar el que mejor calcula la derivada de una función dada. Este documento explica cómo lo hicimos, para qué funciona y qué concluimos.

## Tecnologías usadas
- Matlab Online
- MATLAB

## Setup
Para facilitar la colaboración y la distribución del proyecto se utilizó Matlab Online, al cual se puede acceder desde cualquier ordenador y a través de cualquier explorador siempre y cuando se cuente con una licencia de Matlab.

## Uso
1. Entrar a la página de [Mathworks](https://la.mathworks.com/products/matlab-online.html?requestedDomain=) para poder utilizar Matlab Online.

2.  Hacer click derecho en “Empiece a utilizar MATLAB ONLINE”.![](https://lh6.googleusercontent.com/DLfxB9NrDTFDxw_8eNv1jf5KgeEaBO_BtP2IWhabE9zBM0_r4T6o7UxhOwY_y0PH7kS5-TduKswqoIJEKyNUzhtUi_aalC-PsXyr6akzHgjRqOpykyDMO2touUoQdXI8ZukwUEju)

3.  A continuación se le pedirá ingresar sus datos de acceso para Matlab. En caso de que no cuente con una cuenta de Matlab, deberá crear una. (Es indispensable que cuente con una licencia de Matlab).

4.  Descargar el archivo .mlx del proyecto en su ordenador.

5.  Subir el archivo .mlx en [Matlab Drive.](https://drive.matlab.com/files/) Esto se puede hacer a través de un ‘Drag and Drop’ o, alternativamente, utilizando la opción de “Upload” en la parte superior izquierda. 

![](https://lh3.googleusercontent.com/0LqntlhKPT2cSOximB-Polh_Lle9seDtr14VU5nAcpybSS74j5G1wBRjrVUTmDMPbRel_wFMdMARGfrXVZjMbTKbBL-hS6JbXqD5PLbfa6sszMhMzy-kUOmJE5wpaLknDL7PEI5p)

6.  Regresar Matlab Online y refrescar la página. El proyecto ahora deberá aparecer en la barra izquierda. Haga doble click derecho sobre el proyecto para abrirlo.

![](https://lh3.googleusercontent.com/8jaZAUeQ_02lwLQJRBnbkUVohZY1ZGWmJ4fdTYtkcABnX1e5qqWBb9xs74DdHkoZ5laLwh9BisJZF2GmnIIwHwEMG9bTv62FEob2gOhi0LrrdDLIDy3Fj-88HriLi1gorOPbAAQP)

7.  Para correr el programa, haga click derecho en el botón de “Run” en la barra superior.
![](https://lh5.googleusercontent.com/yzac_8IrQBMM3q9LCNb9mn7Xw8EmhxIvJj3oMQduUBszEsQjxw-p23EkD9Juu63BImn4fAH5pomTbcvKlPyKppp8Xhha71jgGnkZEBhJdUOABHmAAH42-LnSNYhRrk797-7939GN)

8.  Se abrirá una pestaña a la derecha con los resultados del LiveScript. Aquí podrá navegar los resultados y las gráficas de las pruebas realizadas.

## Problemática a resolver
Los métodos de diferenciación son maneras de calcular la derivada de una función. No son tan exactos ni precisos como otros métodos pero se siguen usando en campos matemáticos (e.g. la resolución de ecuaciones diferenciales). Hay diferentes métodos, todos entre ellos parecidos y con pequeñas diferencias entre sí, así como diferentes maneras de calcularlos. Sus resultados son aproximaciones del valor real de la derivada de la función dada. Usamos este proyecto para encontrar el método de diferenciación numérica más exacto.

## Métodos de diferenciación numérica utilizados
Como mencionamos previamente, hay varios métodos de diferenciación numérica. Los tres más comunes son los de diferenciación hacia atrás, diferenciación hacia adelante y diferenciación centrada, llamados así por los valores iniciales que toman. Ahora, las primeras y segundas derivadas hacia adelante, centradas y hacia atrás se pueden calcular usando diferencias finitas o usando coeficientes. Entonces calculamos cuatro funciones por método; como teníamos tres métodos, acabamos con doce funciones en total.

![Diagrama que enseña los tres métodos de diferenciación numérica, las dos formas de calcularlos, y las derivadas que permiten calcular.](https://github.com/luciarenata/proyecto1-com/blob/main/diagrama.png)


La siguiente imagen muestra las fórmulas que utilizamos para calcular, usando diferencias finitas, las primeras derivadas hacia delante, central y hacia atrás.

![Fórmulas de las primeras derivadas usando el método de diferencias finitas.](https://github.com/luciarenata/proyecto1-com/blob/main/formulasDFPD.png)


## Método

Tomamos las fórmulas de diferenciación numérica y las programamos en el lenguaje MATLAB. Revisamos que fueran correctas utilizando la función de derivación de Matlab llamada "diff" y comparándola con nuestro resultado. 

Ejemplo de una gráfica

## Conclusiones
