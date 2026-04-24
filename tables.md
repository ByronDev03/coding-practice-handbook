<h1 align="center">EJERCICIOS DE TABLAS EN HTML5</h1>

---

##### Ejercicio 1. Crea el siguiente horario de clases:
<div align="center">
  <img src="/imgs/tabla1.png" width="600" alt="horario"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horario 1° U</title>
</head>
<body>
    <header>
    	<h1 align="center">HORARIO DE CLASES</h1>
    </header>

     <!--TABLA DATOS-->
    <table border="8" align="center" style="margin-bottom: 20px;">
        <tr>
            <td colspan="3"><strong>CARRERA: </strong> Licenciatura en Informática </td>
        </tr>

        <tr>
            <td colspan="3"><strong>SEMESTRE: </strong> 1° </td>
            <td colspan="3"><strong>GRUPO: </strong> U </td>
            <td colspan="3"><strong>AULA: </strong> 10 </td>
        </tr>

        <tr>
            <td colspan="3"><strong>TURNO: </strong>Matutino</td>
            <td colspan="2"><strong>PERIODO: </strong>Agosto - Diciembre 2021</td>
        </tr>
    </table>

    <!--TABLA HORARIOS-->
    <table border="8" align="center" style="margin-bottom: 20px;">
    	<tr>
    		<th>HORA</th>
    		<th>LUNES</th>
    		<th>MARTES</th>
            <th>MIERCOLES</th>
            <th>JUEVES</th>
            <th>VIERNES</th>
            <th>HORA</th>
    	</tr>

    	<tr>
    		<th>7:00 AM / 7:50 AM</th>
            <td align="center"></td>
            <td align="center">Contabilidad Financiera</td>
            <td align="center">Introducción a la Programación</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">Contabilidad Financiera</td>
            <th>7:00 AM / 7:50 AM</th>
    	</tr> 

    	<tr>
    		<th>7:50 AM / 8:40 AM</th>
            <td align="center">Contabilidad Financiera</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">Contabilidad Financiera</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">Contabilidad Financiera</td>
            <th>7:50 AM / 8:40 AM</th>
    	</tr>

    	<tr>
    		<th>8:40 AM / 9:30 AM</th>
            <td align="center">Introducción a la Programación</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">UATM: Aprendizaje Estratégico</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">UATM: Aprendizaje Estratégico</td>
            <th>8:40 AM / 9:30 AM</th>
    	</tr>

    	<tr>
    		<th>9:30 AM / 9:50 AM</th>
            <td colspan="5" align="center"><strong >R E C E S O</strong></td>
            <th>9:30 AM / 9:50 AM</th>
    	</tr>

    	<tr>
    		<th>9:50 AM / 10:40 AM</th>
            <td align="center">Administración</td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center"></td>
            <td align="center">Introducción a la Programación</td>
            <th>9:50 AM / 10:40 AM</th>
    	</tr>

    	<tr>
    		<th>10:40 AM / 11:30 AM</th>
            <td align="center">Administración</td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center">Introducción a la Programación</td>
            <td align="center"></td>
            <th>10:40 AM / 11:30 AM</th>
    	</tr>

    	<tr>
    		<th>11:30 AM / 12:20 PM</th>
            <td align="center">Tutoría</td>
            <td align="center"><em>Inglés Básico</em></td>
            <td align="center"><em>Inglés Básico</em></td>
            <td align="center">Introducción a la Programación</td>
            <td align="center">Administración</td>
            <th>11:30 AM / 12:20 PM</th>
    	</tr>

    	<tr>
    		<th>12:20 PM / 13:10 PM</th>
            <td align="center">UATM: Aprendizaje Estratégico</td>
            <td align="center"></td>
            <td align="center">Administración</td>
            <td align="center"><em>Inglés Básico</em></td>
            <td align="center"></td>
            <th>12:20 PM / 13:10 PM</th>
    	</tr>

        <tr>
    		<th>13:10 PM / 14:00 PM</th>
            <td align="center">UATM: Aprendizaje Estratégico</td>
            <td align="center"></td>
            <td align="center">Administración</td>
            <td align="center"></td>
            <td align="center"></td>
            <th>13:10 PM / 14:00 PM</th>
    	</tr>

        <tr>
    		<th>14:00 PM / 14:50 PM</th>
            <td align="center"></td>
            <td align="center"></td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center"></td>
            <td align="center">UATM: Aprendizaje Estratégico</td>
            <th>14:00 PM / 14:50 PM</th>
    	</tr>
    </table>
 
     <!--TABLA CATEDRATICOS-->
    <table border="8" align="center">
        <tr>
    		<th>CLAVE</th>
    		<th>ASIGNATURA</th>
    		<th>HORAS</th>
            <th>CATEDRÁTICO</th>
    	</tr>

        <tr>
            <td align="center">MBC-01</td>
            <td align="center">Matemáticas Básicas para la Computación</td>
            <td align="center">5</td>
            <td align="center">Ing. </td>
    	</tr> 

        <tr>
            <td align="center">IP-02</td>
            <td align="center">Introducción a la Programación</td>
            <td align="center">5</td>
            <td align="center">Ing. </td>
    	</tr> 

        <tr>
            <td align="center">CF-03</td>
            <td align="center">Contabilidad Financiera</td>
            <td align="center">5</td>
            <td align="center">Lic. </td>
    	</tr> 

        <tr>
            <td align="center">AD-04</td>
            <td align="center">Administración</td>
            <td align="center">5</td>
            <td align="center">Mtro. </td>
    	</tr> 

        <tr>
            <td align="center">EPO-05</td>
            <td align="center">Ética Profesional en las Organizaciones</td>
            <td align="center">5</td>
            <td align="center">Mtra. </td>
    	</tr> 

        <tr>
            <td align="center">UATMAE-06</td>
            <td align="center">Unidad de Aprendizaje Transversal Multimodal: Aprendizaje Estratégico</td>
            <td align="center">5</td>
            <td align="center">Mtro. </td>
    	</tr> 

        <tr>
            <td align="center">IB-07</td>
            <td align="center"><em>Inglés Básico</em></td>
            <td align="center"><em>3</em></td>
            <td align="center"><em>Lic. </em></td>
    	</tr> 

        <tr>
            <td align="center">TTA1-08</td>
            <td align="center">Tutoría</td>
            <td align="center">1</td>
            <td align="center">Ing. </td>
    	</tr> 
    </table>
</body>
</html>
```
</details>


##### Ejercicio 2. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla2.png" width="300" alt="tabla"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 2</title>
</head>
<body>
    <table border="1">
        <caption>Titulo de la tabla</caption>
        <tr>
            <th>Col.Cab 1</th>
            <th>Col.Cab 2</th>
        </tr>
        <tr>
            <td>Celda 1</td>
            <td>Celda 2</td>
        </tr>
    </table>
</body>
</html>
```
</details>


##### Ejercicio 3. Crea la siguiente tabla con combinacion de columnas:
<div align="center">
  <img src="/imgs/tabla3.png" width="400" alt="tabla con combinación de columnas"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 3</title>
</head>
<body>
    <table border="1">
        <caption>Tabla con combinación de columnas</caption>
        <tr>
            <th colspan="2">Celda Combinada</th>
            <th>Celda Normal</th>
            <th colspan="2">Celda Combinada</th>
        </tr>
        <tr>
            <td>C1</td>
            <td>C2</td>
            <td>C3</td>
            <td>C4</td>
            <td>C5</td>
        </tr>
        <tr>
            <td>C6</td>
            <td>C7</td>
            <td>C8</td>
            <td colspan="2">C9 Comb.</td>
        </tr>
    </table>
</body>
</html>
```
</details>


##### Ejercicio 4. Crea la siguiente tabla con combinacion de filas:
<div align="center">
  <img src="/imgs/tabla4.png" width="400" alt="tabla con combinación de filas"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 4</title>
</head>
<body>
    <table border="1">
        <caption>Tabla con combinación de filas</caption>
        <tr>
            <th>Celda 1</th>
            <th>Celda 2</th>
            <th>Celda 3</th>
        </tr>
        <tr>
            <td rowspan="2">Celda combinada</td>
            <td>Celda 5</td>
            <td rowspan="2">Celda combinada</td>
        </tr>
        <tr>
            <td>Celda 7</td>
        </tr>
    </table>
</body>
</html>
```
</details>


##### Ejercicio 5. Crea la siguiente tabla con combinacion de filas y columnas:
<div align="center">
  <img src="/imgs/tabla5.png" width="300" alt="tabla combinada de filas y columas"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 5</title>
</head>
<body>
    <table border="1">
        <caption>Tabla con combinación de filas y columnas</caption>
        <tr>
            <th>Celda 1</th>
            <th>Celda 2</th>
            <th>Celda 3</th>
            <th>Celda 4</th>
        </tr>
        <tr>
            <td rowspan="3">Celda 5</td>
            <td>Celda 6</td>
            <td colspan="2">Celda 7</td>
        </tr>
        <tr>
            <td>Celda 8</td>
            <td>Celda 9</td>
            <td rowspan="2">Celda 10</td>
        </tr>
        <tr>
            <td colspan="2">Celda 11</td>
        </tr>
    </table>
</body>
</html>
```
</details>


##### Ejercicio 6. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla6.png" width="400" alt="tabla"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 6</title>
</head>
<body>
    <table border="1">
        <caption>Titulo de la tabla</caption>
        <colgroup>
            <col style="width: 20%"/>
            <col style="width: 40%"/>
            <col style="width: 60%"/>
        </colgroup>
        <thead>
            <tr>
                <th rowspan="2">Tabla Avanzada</th>
                <th colspan="2">Cabecera Múltiples Columnas</th>
            </tr>
            <tr>
                <th>Primera Col. Cab.</th>
                <th>Segunda Col. Cab.</th>
            </tr>
        </thead>
        <tfoot>
            <tr>
                <td colspan="3">Pie de Tabla.</td>
            </tr>
        </tfoot>
        <tbody>
            <tr>
                <th>Fila 1</th>
                <td>Fila 1 Columna 1</td>
                <td>Fila 1 Columna 2</td>
            </tr>
            <tr>
                <th>Fila 2</th>
                <td>Fila 2 Columna 1</td>
                <td>Fila 2 Columna 2</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```
</details>


##### Ejercicio 7. Crea la siguiente tabla usa las fusiones de columnas y filas:
<div align="center">
  <img src="/imgs/tabla7.png" width="100" alt="tabla"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 7</title>
</head>
<body>
    <table border="1">
        <tr>
            <td colspan="2">A</td>
            <td>B</td>
            <td>C</td>
        </tr>
        <tr>
            <td rowspan="3">D</td>
            <td colspan="2">E</td>
            <td>F</td>
        </tr>
        <tr>
            <td>G</td>
            <td colspan="2">H</td>
        </tr>
        <tr>
            <td>I</td>
            <td>J</td>
            <td>K</td>
        </tr>
    </table>
</body>
</html>
```
</details>


#### Ejericicio 8. Crea una tabla con el siguinete aspecto:
<div align="center">
  <img src="/imgs/tabla8.png" width="150" alt="tabla medallas"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 8</title>
</head>
<body>
    <table border="1">
    <caption>Medallas olimpicas</caption>
    <tr>
        <th>Paises</th>
        <th>Medallas</th>
    </tr>
    <tr>
        <td>USA</td>
        <td>13</td>
    </tr>
    <tr>
        <td>China</td>
        <td>25</td>
    </tr>
    <tr>
        <td>España</td>
        <td>3</td>
    </tr>
    <tr>
        <td>Francia</td>
        <td>6</td>
    </tr>
    </table>
</body>
</html>
```
</details>


#### Ejericio 9. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla9.png" width="300" alt="tabla pib"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 9</title>
</head>
<body>
    <table border="1">
    <tr>
        <th>Mes</th>
        <td>Enero</td>
        <td>Febrero</td>
        <td>Marzo</td>
        <td>Abril</td>
        <td>Mayo</td>
        <td>Junio</td>
    </tr>
    <tr>
        <th>PIB</th>
        <td>0.2</td>
        <td>0.4</td>
        <td>0.2</td>
        <td>0.3</td>
        <td>0.1</td>
        <td>0.2</td>
    </tr>
    <tr>
        <th>PNIB</th>
        <td>1.3</td>
        <td>1.2</td>
        <td>1.1</td>
        <td>1.9</td>
        <td>1.7</td>
        <td>1.6</td>
    </tr>
    </table>
</body>
</html>
```
</details>


#### Ejericio 10. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla10.png" width="200" alt="tabla empleado"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 10</title>
</head>
<body>
    <table border="1">
        <tr>
            <th>Empleado</th>
            <th>Información</th>
        </tr>

        <tr>
            <td>Juan</td>
            <td>
                <table border="1">
                <tr>
                    <td>Edad</td>
                    <td>30</td>
                </tr>
                <tr>
                    <td>Área</td>
                    <td>Backend</td>
                </tr>
                </table>
            </td>
        </tr>
    </table>
</body>
</html>
```
</details>


#### Ejericio 11. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla11.png" width="300" alt="tabla promedio"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 11</title>
</head>
<body>
    <table border="1">
        <tr>
            <th rowspan="2">Alumno</th>
            <th colspan="3">Calicaciones</th>
        </tr>
        <tr>
            <th>Español</th>
            <th>Matematicas</th>
            <th>Promedio</th>
        </tr>
        <tr>
            <td>Mario</td>
            <td>10</td>
            <td>8</td>
            <td>9</td>
        </tr>
    </table>
</body>
</html>
```
</details>

#### Ejericio 12. Crea la siguiente tabla:
<div align="center">
  <img src="/imgs/tabla12.png" width="300" alt="tabla productos"/>
</div>

<details>
<summary>Solución</summary>

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 12</title>
</head>
<body>
    <table border="1">
        <thead>
            <tr>
                <th>Producto</th>
                <th>Precio</th>
                <th>Cantidad</th>
                <th>Total</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Laptop</td>
                <td>10,000</td>
                <td>2</td>
                <td>20,000</td>
            </tr>
            <tr>
                <td>Mouse</td>
                <td>200</td>
                <td>3</td>
                <td>600</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td colspan="3"><strong>Total General</strong></td>
                <td><strong>20,600</strong></td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
```
</details>