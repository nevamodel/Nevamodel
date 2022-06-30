<title><b>Herramienta para el cálculo de la carga de nieve sobre terreno horizontal</b></title>


El modelo de cálculo que se presenta se ha desarrollado bajo las siguientes premisas:
- Cada hoja del libro tiene título.
- Cada bloque que se analice dentro de una hoja tiene título.
- Formato de las celdas de entrada de datos: fondo gris y texto negro. 
  Este formato se emplea exclusivamente cuando se introducen datos a partir de los que se realiza el estudio. 
  Es decir, los datos de la serie histórica de AEMET son los que adoptan este formato.
- Formato de las celdas de enlace: este tipo de celdas, se presentan con fondo con RGB 238; 236; 225, y texto de color azul. 
-	Formato de las celdas de cálculo: se presentan con el mismo fondo de las celdas de enlace y texto negro.
-	Formato de las celdas de hipótesis: se muestran con fondo amarillo y texto rojo. 
  Se trata de las únicas celdas en las que el usuario puede variar las hipótesis de cálculo.
 
![image](https://user-images.githubusercontent.com/108299903/176739536-bcb721d4-7ed8-40b0-b4ca-25729b050395.png)

<b><H2>Manual de Instrucciones</H2><b>

- Pestaña Datos y Cálculos: 
  - Introducir en el bloque 1 - Datos de Partida, los datos de AEMET de la estación meteorológica selecionada.
  - Identificar en las Celdas de Hipótesis los datos relativos a la estación (nombre, altitud) y las fechas sobre las que se quiere realizar la consulta.
  - Ejecutar las macros mediante los botones Listar y a continuación Cálculos.
  
- Pestaña Simulación de Montecarlo:
  - Ejecutar la macro Simulación mediante el botón disponible. 
 
- Pestaña Análisis y Resultados:
  - En el gráfico 1 se deben  excluir los valores cero de la precipitación simulada.
  - Seleccionar la línea de tendencia más adecuada, preferiblemente con R2 >0,9
  - Los parámetros A y B se determinan a partir de la fórmula de regresión  del gráfico 1: Y= A*Ln(x)+B
  - La fórmula de regresión se emplea solo si la precipitación simulada es = 0
  - El gráfico 2 es el resultado final.
  - La sobrecarga de nieve se calcula en el bloque 8 - Resultados, seleccionando un Periodo de Retorno y un Peso Específico.

- Pestaña Función de Probabilidad:
  - Se puede consultar esta función y se refrescan los datos mediante el botón Actualizar.

