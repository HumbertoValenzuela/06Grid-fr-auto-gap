# 06Grid-fr-auto-gap
* 06 Grid Formas para usar grid-template-columns: repeat(3, 1fr); grid: auto / 1fr;

```javascript
.servicios {
    border: 3px solid black;
    height: 300px;
    display: grid;
/* formas indicar columnas usando grid template-columns */
grid-template-columns: 33.3% 33.3% 33.3%;
grid-template-columns: repeat(3, 33.3%);
/* fracciones. en este caso tendra una tercera parte */
grid-template-columns: 1fr 1fr 1fr;
grid-template-columns: repeat(3, 1fr);
/* dos fracciones de las cuatro y los dos últimos 1/4 cada uno*/
grid-template-columns: 2fr 1fr 1fr;
grid-template-columns: 2fr repeat(2, 1fr);
/* tendra dos filas */
grid-template-rows: 1fr 1fr;
grid-template-rows: 50% 50%;
grid-template-rows: repeat(2, 1fr);
/* primera fila medir el 75% y el resto 25% */
grid-template-rows: 3fr 1fr;
/*Lo mismo usando shorthand grid. row / column */
grid: repeat(2, 1fr) / repeat(3, 1fr);
/* No definir Row(ignora el primer parametro) y si columnas */
grid: auto / repeat(3, 1fr);    
}

/* gap */
.servicios1 {
    border: 3px solid black;
    height: 300px;
    display: grid;

/* No definir Row(ignora el primer parametro).pero si el contenedor */
/* tiene mas div este los creará automaticamente */
grid: auto / repeat(3, 1fr);  
row-gap: 1rem;  
column-gap: 1rem;
gap: 1rem;
}
```
