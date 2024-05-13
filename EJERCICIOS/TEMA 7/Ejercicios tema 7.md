# Ejercicios tema 7

## Árboles de decisión

### Ejemplo 1

Una empresa está analizando tres mejoras posibles. La primera es ampliar en número de operarios. La segunda una mejora en la maquinaria utilizada y la tercera no llevar a cabo ningún cambio. La tabla siguiente muestra los beneficios correspondientes y sus probabilidades en función de la demanda del producto.

<table>
  <tr style="background-color: rgb(0, 147, 255);color:#FFFFFF">
    <th><center>Mejora</center></th>
    <th><center>Demanda alta</center></th>
    <th><center>p</center></th>
    <th><center>Demanda media</center></th>
    <th><center>p</center></th>
  </tr>
  <tr>
    <td><center>1</center></td>
    <td><center>200000€</center></td>
    <td><center>0,6</center></td>
    <td><center>70000€</center></td>
    <td><center>0,4</center></td>
  </tr>
  <tr>
    <td><center>2</center></td>
    <td><center>180000€</center></td>
    <td><center>0,4</center></td>
    <td><center>160000€</center></td>
    <td><center>0,6</center></td>
  </tr>
  <tr>
    <td><center>3</center></td>
    <td><center>150000€</center></td>
    <td><center>0,2</center></td>
    <td><center>140000€</center></td>
    <td><center>0,8</center></td>
  </tr>
</table>


#### Pasos

1. **Partimos de la situación inicial**.

2. **Se agregan los nodos de mejora**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_1_2.png?raw=true" alt="Arbol_decision_paso_1_2.png" style="zoom:25%;" />

3. **Se expande el diagrama hasta llegar a los puntos finales**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_3.png?raw=true" alt="Arbol_decision_paso_3.png" style="zoom:25%;" />

   

4. **Se calculan los valores del árbol**.

   $\mathbf{\color{blue}Valor\ esperado\ (EV)} = (primer\ resultado\ posible * {\color{red}probabilidad\ del\ resultado}) + (segundo\ resultado\ posible * {\color{red}probabilidad\ del\ resultado}) - costo$

   

   $\mathbf{\color{blue}EV_1} = (200000 * {\color{red}0,6}) + (70000 * {\color{red}0,4}) - 0 = 120000 + 28000 = \mathbf{148000}$

   $\mathbf{\color{blue}EV_2} = (180000* {\color{red}0,4}) + (160000* {\color{red}0,6}) - 0 = 72000 + 96000 = \mathbf{168000}$

   $\mathbf{\color{blue}EV_3} = (150000* {\color{red}0,2}) + (140000 * {\color{red}0,8}) - 0 = 30000 + 112000 = \mathbf{142000}$

   

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_4.png?raw=true" alt="Arbol_decision_paso_4.png" style="zoom:25%;" />

   

5. **Se evalúan los resultados**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_5.png?raw=true" alt="Arbol_decision_paso_5.png" style="zoom:25%;" />

   

   Por lo tanto, **se decide aplicar la mejora 2**.



### Ejemplo 2

Hay que decidir sobre el cierre o permanencia de una sucursal de nuestra empresa en Turquía.

La valoración desde el punto de vista de cuantificación de los resultados sería la siguiente:

- Sucursal con beneficios: +100.
- Sucursal sin pérdidas: +50.
- Sucursal con pérdidas: -100.

En caso de que se decida continuar con la sucursal abierta es posible que a corto plazo Turquía se integre en la UE (50% Prob). En ese supuesto se estima que con un 60% de probabilidad se podrían recibir ayudas económicas para incentivar el desarrollo tecnológico en el país, lo que supondría un incremento en los beneficios de la empresa. En caso de no recibir las ayudas se estima que la sucursal podría mantenerse sin pérdidas.

Si Turquía no se integra en la UE se estima que con un 70% de probabilidad aumentaría la inseguridad ciudadana (revueltas, atentados…), lo que desincentivaría el consumo e implicaría que nuestra sucursal tuviera pérdidas. Si no aumentase la inseguridad ciudadana la sucursal podría mantenerse sin pérdidas.

En el caso de que decidiésemos cerrar la sucursal, se estima una probabilidad de reubicación en otras sedes de los recursos humanos y materiales del 70%, por lo que no se imputarían pérdidas a la sucursal. En caso contrario se estimaría un cierre con pérdidas.



#### Pasos

1. **Partimos de la situación inicial**.

2. **Se agregan los nodos de mejora**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_1_2_ejercicio_2.png?raw=true" alt="Arbol_decision_paso_1_2_ejercicio_2.png" style="zoom: 25%;" />

   

3. **Se expande el diagrama hasta llegar a los puntos finales**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_3_ejercicio_2.png?raw=true" alt="Arbol_decision_paso_3_ejercicio_2.png" style="zoom:25%;" />

   

4. **Se calculan los valores del árbol**.

   $\mathbf{\color{blue}Valor\ esperado\ (EV)} = (primer\ resultado\ posible * {\color{red}probabilidad\ del\ resultado}) + (segundo\ resultado\ posible * {\color{red}probabilidad\ del\ resultado}) - costo$

   

   $\mathbf{\color{blue}EV_3} = (100 * {\color{red}0,6}) + (50 * {\color{red}0,4}) - 0 = 60 + 20 = \mathbf{80}$

   $\mathbf{\color{blue}EV_4} = (-100 * {\color{red}0,7}) + (50 * {\color{red}0,3}) - 0 = -70 + 15 = \mathbf{-55}$​

   

   $\mathbf{\color{blue}EV_1} = (80 * {\color{red}0,5}) + (-55 * {\color{red}0,5}) - 0 = 40 - 27,5 = \mathbf{12,5}$

   $\mathbf{\color{blue}EV_2} = (50 * {\color{red}0,7}) + (-100 * {\color{red}0,3}) - 0 = 35 - 30 = \mathbf{5}$

   

   

   <img src="images/Arbol_decision_paso_4_ejercicio_2.png" alt="Arbol_decision_paso_4_ejercicio_2" style="zoom:25%;" />

   

   

5. **Se evalúan los resultados**.

   

   <img src="https://github.com/JMPinillos/Integracion_sistemas-UNIR/blob/main/EJERCICIOS/TEMA%207/images/Arbol_decision_paso_5_ejercicio_2.png?raw=true" alt="Arbol_decision_paso_5_ejercicio_2.png" style="zoom:25%;" />

   

   Por lo tanto, **se decide mantener la sucursal abierta**.

