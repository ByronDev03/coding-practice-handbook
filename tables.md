<h1 align="center">EJERCICIOS DE TABLAS EN HTML5</h1>

##### Ejercicio 1. Recrea el siguinte horario de clases
<div align="center">
  <img src="/imgs/horario1.png" width="600" alt="Diagrama cliente-servidor" />
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