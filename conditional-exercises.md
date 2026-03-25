<h1 align="center">EJERCICIOS DE CONDICIONALES</h1>

---

##### Ejercicio 1. Crear un programa que calcule si un número es par o impar
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_1
	Definir Num Como Entero
	Num <- 0; 
	
	Escribir "------PROGRAMA QUE CALCULA SI UN NUMERO ES PAR O IMPAR------";
	Escribir "Ingrese un numero: ";
	Leer Num;
	
	Si (Num % 2 == 0) Entonces
		Escribir "El numero ",Num," es PAR";
	SiNo
		Escribir "El numero ",Num," es IMPAR";
	FinSi	
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++

```
</details>

##### Ejercicio 2. Crear un programa que calcule si un número es múltiplo de 2,3 o 4, en el caso contrario imprimir número invalido
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_2
	Definir Num Como Entero
	Num <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA EL MULTIPLO DE 2 o 3------";
	Escribir "Ingrese un numero: ";
	Leer Num;
	
	Si (Num % 2 == 0) Entonces
		Escribir "El numero ingresado ",Num," es MULTIPLO DE 2";
	FinSi
	Si (Num % 3 == 0) Entonces
		Escribir "El numero ingresado ",Num," es MULTIPLO DE 3";
	FinSi
	
	Si (Num % 2 <> 0 o Num % 3 <> 0) Entonces
		Escribir "El numero ingresado ",Num," es INVALIDO POR NO SER MULTIPLO DE 2 O 3";
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++

```
</details>

##### Ejercicio 3. Crear un programa que lea la altura e imprima en pantalla si la persona tiene una altura promedio, alta o baja. Tomando en cuenta lo siguiente:
| ALTO        |   PROMEDIO    |    BAJO    |
| :---:       |     :---:     |    :--:    |
| 1.80 o mas  |  1.60 a 1.79  |  0 a 1.59  | 
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_3
	Definir estatura Como Real
	estatura <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA LA ESTATURA DE UNA PERSONA------";
	Escribir "Ingrese su estatura: ";
	Leer estatura;
	
	Si (estatura >= 0 y estatura <= 1.59) Entonces 
		Escribir "Su estatura ingresada ",estatura," es BAJA";
	FinSi
	Si (estatura >= 1.60 y estatura <= 1.79) Entonces 
		Escribir "Su estatura ingresada ",estatura," es PROMEDIO";
	FinSi
	Si (estatura >= 1.80) Entonces 
		Escribir "Su estatura ingresada ",estatura," es ALTA";
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void EstaturaPersona()
{
	float estatura = 0;
	cout<<"\t---PROGRAMA QUE CALCULA LA ESTATURA DE UNA PERSONA---"<<endl;
	cout<<"Ingrese su estatura: ";
	cin>>estatura;
	system("cls");
	if(estatura >= 0 && estatura <= 1.59)
	cout<<"SU ESTATURA INGRESADA "<<estatura<<" ES BAJA"<<endl;
	if(estatura >= 1.60 && estatura <= 1.79)
	cout<<"SU ESTATURA INGRESADA "<<estatura<<" ES PROMEDIO"<<endl;
	if(estatura >= 1.80)
	cout<<"SU ESTATURA INGRESADA "<<estatura<<" ES ALTA"<<endl;
	
}
int main()
{
	system("color 0A");
	EstaturaPersona();
	return 0;
}
```
</details>

##### Ejercicio 4. Determinar si un alumno aprueba o reprueba un curso, sabiendo que aprobara si su promedio de tres calificaciones es mayor o igual a 7; reprueba en caso contrario
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_4
	Definir Cal1, Cal2, Cal3 Como Entero
	Definir promedio Como Real
	Cal1 <- 0;
	Cal2 <- 0;
	Cal3 <- 0;
	promedio <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA SI UN ALUMNO ESTA APROBADO O NO------";
	Escribir "Ingrese la primer calificaci�n obtenida: ";
	Leer Cal1;
	Escribir "Ingrese la segunda calificaci�n obtenida: ";
	Leer Cal2;
	Escribir "Ingrese la tercera calificaci�n obtenida: ";
	Leer Cal3; 
	
	promedio <- (Cal1+Cal2+Cal3)/3;
	
	Si (promedio >= 7) Entonces
		Escribir "La calificaci�n obtenida de ",promedio," es APROBATORIA";
	SiNo
		Escribir "La calificaci�n obtenida de ",promedio," es REPROBATORIA";
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int Cal1 = 0, Cal2 = 0, Cal3 = 0;
float promedio = 0;
void EntradaDatos()
{
	cout<<"\t---PROGRAMA QUE CALCULA SI UN ALUMNO ESTA APROBADO O NO---"<<endl;
	cout<<"Ingrese la primer calificacion obtenida: ";
	cin>>Cal1;
	cout<<"Ingrese la segunda calificacion obtenida: ";
	cin>>Cal2;
	cout<<"Ingrese la tercer calificacion obtenida: ";
	cin>>Cal3;
	system("cls");
}
void AprobadoReprobado()
{
	EntradaDatos();
	promedio = (Cal1 + Cal2 + Cal3) / 3;
	if(promedio >= 7)
	cout<<"LA CALIFICACIÓN OBTENIDA "<<promedio<<" ES APROBATORIA"<<endl;
	else
	cout<<"LA CALIFICACIÓN OBTENIDA "<<promedio<<" ES REPROBATORIA"<<endl;
}
int main() 
{
	system("color 0A");
	AprobadoReprobado();
	return 0;
}
```
</details>

##### Ejercicio 5. Calcular el interés ganado mensualmente si una persona invierte en un banco, y este paga un interés mensual del 2% si la inversión es mayor o igual a 10,000 o un 3% si la inversión es mayor o igual a 20,000 o un 5% si la inversión es mayor o igual a 40,000
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_5
	Definir inver,ints Como Entero
	inver <- 0;
	ints <- 0;
	Escribir "------PROGRAMA QUE CALCULA EL INTERES GANADO MENSUALMENTE------";
	Escribir "Ingrese su inversión: ";
	Leer inver;
	Si (inver >= 0 y inver < 10000) Entonces
		ints <- 0;
	FinSi
	Si (inver >= 10000 y inver < 20000) Entonces
		ints <- inver * 0.02;
	FinSi
	Si (inver >= 20000 y inver < 40000) Entonces
		ints <- inver * 0.03;
	FinSi
	Si (inver >= 40000) Entonces
		ints <- inver * 0.05;
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "Su interes mensual es de $",ints," por la inversion de: $",inver;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int inver = 0, ints = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"SU INTERES MENSUAL ES DE $"<<ints<<" POR LA INVERSION DE: $"<<inver;
}
void CalcularInteres()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL INTERES GANADO MENSUALMENTE---"<<endl;
	cout<<"Ingrese su inversion: $";
	cin>>inver;
	if(inver >= 0 && inver < 10000)
	ints = 0;
	if(inver >= 10000 && inver < 20000)
	ints = inver * 0.02;
	if(inver >= 20000 && inver < 40000)
	ints = inver * 0.03;
	if(inver >= 40000)
	ints = inver * 0.05;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	CalcularInteres();
	return 0;
}
```
</details>

##### Ejercicio 6. En un almacén se hace un 5% de descuento a los clientes cuya compra supere los $6,000.00 o un 10% si la compra supera los $8,000.00 ¿Cuál será la cantidad que pagara una persona por su compra y cuál es su descuento?
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_6
	Definir mtocompra, descuento, total_compra Como Entero
	mtocompra <- 0;
	descuento <- 0;
	total_compra <- 0;
	Escribir "----PROGRAMA QUE CALCULA EL DESCUENTO EN UN ALMACÉN----";
	Escribir "Ingrese el monto de la compra: ";
	Leer mtocompra;
	Si (mtocompra > 6000) Entonces
		descuento <- mtocompra * 0.05;
	SiNo
		Si (mtocompra > 8000)  Entonces
			descuento <- mtocompra * 0.10;
		FinSi
	FinSi
	total_compra <- mtocompra - descuento;
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "Por el monto de compra de ",mtocompra," el total a pagar es de: $",total_compra;	
	Escribir "El descuento aplicado es de: $",descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int mtocompra = 0, descuento = 0, TotalCompra = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL TOTAL A PAGAR ES DE: $"<<TotalCompra<<endl;
	cout<<"DESCUENTO APLICADO: $"<<descuento<<endl;
}
void DescuentoAlmacen()
{
    cout<<"\t---PROGRAMA QUE CALCULA EL DESCUENTO EN UN ALMACEN---"<<endl;
	cout<<"Ingrese el monto de la compra: $";
	cin>>mtocompra;
	if(mtocompra > 6000)
	descuento = mtocompra * 0.05;
	if(mtocompra > 8000)
	descuento = mtocompra * 0.10;
	
	TotalCompra = mtocompra - descuento;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	DescuentoAlmacen();
	return 0;
}
```
</details>

##### Ejercicio 7. Un obrero necesita calcular su salario semanal, el cual se obtiene de la siguiente manera:
- Si trabaja 40 horas o menos se le paga $16 por hora
- Si trabaja más de 40 horas se le paga $20 por hora extra trabajada.
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_7
	Definir hrstrab,hrsextras,sueldo_semanal Como Real
	hrstrab <- 0;
	hrsextras <- 0;
	salario_semanal <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA EL SALARIO SEMANAL DE UN OBRERO------";
	Escribir "Ingrese sus horas trabajadas: ";
	Leer hrstrab;
	
	Si (hrstrab > 40) Entonces
		hrsextras <- hrstrab - 40;
		salario_semanal <- (hrsextras * 20) + (40 * 16);
	SiNo
		salario_semanal <- hrstrab * 16;
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El salario semanal que persive por ",hrstrab," horas trabajadas es de: $",salario_semanal;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int hrstrab = 0, hrsextras = 0;
float SalSem = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL SALARIO SEMANAL QUE PERSIVE POR "<<hrstrab<<" HORAS TRABAJADAS ES DE: $"<<SalSem;
}
void SalarioObrero()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL SALARIO SEMANAL DE UN OBRERO---"<<endl;
	cout<<"Ingrese sus horas trabajadas: ";
	cin>>hrstrab;
	if(hrstrab > 40)
	{
		hrsextras = hrstrab - 40;
		SalSem = (hrsextras * 20) + (40 * 16);
	}
	else
	SalSem = hrstrab * 16;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	SalarioObrero();
	return 0;
}
```
</details>

##### Ejercicio 8. Programa que lea dos números y los imprima en forma ascendente.
- Ejemplo:
    - 1
    - 5
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_8
	Definir Num1, Num2 Como Entero
	Num1 <- 0;
	Num2 <- 0;
	
	Escribir "------PROGRAMA QUE ORDENA NUMEROS INGRESADOS DE FORMA ASCENDENTE-----";
	Escribir "Ingrese el primer numero: ";
	Leer Num1;
	Escribir "Ingrese el segundo numero: ";
	Leer Num2;
	
	Si (Num1 < Num2) Entonces
		Escribir Num1;
		Escribir Num2;
	SiNo
		Escribir Num2;
		Escribir Num1;
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void NumerosAscendentes()
{
	int num1 = 0, num2 = 0;
	cout<<"\t---PROGRAMA QUE ORDENA NUMEROS INGRESADOS DE FORMA ASCENDENTE---"<<endl;
	cout<<"Ingrese el primer numero: ";
	cin>>num1;
	cout<<"Ingrese el segundo numero ";
	cin>>num2;
	system("cls");
	if(num1 < num2)
	{
	  cout<<num1<<endl;
	  cout<<num2<<endl;	
	}
	else
	{
	  cout<<num2<<endl;
	  cout<<num1<<endl;	
	}
}
int main()
{
	system("color 0A");
	NumerosAscendentes();
	return 0;
}
```
</details>

##### Ejercicio 9. Hacer un programa que calcule el total a pagar por la compra de camisas. Si se compran tres camisas o más se aplica un descuento del 20% sobre el total de la compra y si son menos de tres camisas un descuento del 10%
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_9
	Definir numcam,descuento,total_pagar,precam Como Entero 
	numcam <- 0; 
	descuento <- 0;
	total_pagar <- 0;
	precam <- 0;
	Escribir "----PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR UNAS CAMISAS----";
	Escribir "Ingrese el numero de camisas a comprar: ";
	Leer numcam;
	Escribir "Ingrese el precio de las camisas: ";
	Leer precam;
	total_pagar <- numcam * precam;
	Si (numcam > 3) Entonces
		descuento <- total_pagar * 0.20;
	SiNo
		Si (numcam < 3) Entonces
			descuento <- total_pagar * 0.10;
		FinSi
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El total a pagar por ",numcam," camisas compradas es de: $",total_pagar - descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int numcam = 0, precam = 0; 
float TotalPagar = 0, descuento = 0, subtotal = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL TOTAL A PAGAR POR "<<numcam<<" CAMISAS COMPRADAS ES DE: $"<<TotalPagar;	
}
void PagoCamisas()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR UNAS CAMISAS---"<<endl;
	cout<<"Ingrese el numero de camisas a comprar: ";
	cin>>numcam;
	cout<<"Ingrese el precio de las camisas: $";
	cin>>precam;
	subtotal = numcam * precam;
	system("cls");
	if(numcam > 3)
	descuento = subtotal * 0.20;
	else
	descuento = subtotal * 0.10;
	
	TotalPagar = subtotal - descuento;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	PagoCamisas();
	return 0;
}
```
</details>

##### Ejercicio 10. Calcular el total que una persona debe pagar en una llantera, si el precio de cada llanta es de $800 si se compran menos de 5 llantas y de $700 si se compran 5 o más
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_10
	Definir numllantas, pago_total Como Entero
	numllantas <- 0;
	pago_total <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA EL TOTAL A PAGAR EN UNA LLANTERA------";
	Escribir "Ingrese el numero de llantas a comprar: ";
	Leer numllantas;
	
	Si (numllantas < 5) Entonces
		pago_total <- numllantas * 800; 
	SiNo
		pago_total <- numllantas * 700;
	FinSi
	
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El pago total por ",numllantas," llantas compradas es de: $",pago_total;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int numllantas = 0, PagoTotal = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL PAGO TOTAL POR "<<numllantas<<" LLANTAS COMPRADAS ES DE: $"<<PagoTotal;
}

void Llantera()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR EN UNA LLANTERA---"<<endl;
	cout<<"Ingrese las llantas a comprar: ";
	cin>>numllantas;
	if(numllantas < 5)
	PagoTotal = numllantas * 800;
	else
	PagoTotal = numllantas * 700;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	Llantera();
	return 0;
}
```
</details>

##### Ejercicio 11. En un almacén se hace un 20% de descuento a los clientes cuya compra supere los $1000 ¿Cuál será la cantidad que pagara una persona por su compra?
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_11
	Definir mtocompra,descuento Como Entero
	mtocompra <- 0;
	descuento <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR UN 20% DE DESCUENTO------";
	Escribir "Ingrese el monto de la compra: ";
	Leer mtocompra;
	
	Si (mtocompra > 1000) Entonces
		descuento <- mtocompra * 0.20;
	SiNo
		descuento = 0;
	FinSi
	pago_total <- mtocompra - descuento;
	Escribir "La cantidad total que pagara por ",mtocompra," es de: $",pago_total;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int mtocompra = 0, descuento = 0;
float PagoTotal = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"LA CANTIDAD A PAGAR POR $"<<mtocompra<<" ES DE: $"<<PagoTotal;
}
void Descuento()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR UN 20% DE DESCUENTO---"<<endl;
	cout<<"Ingrese el monto de la compra: $";
	cin>>mtocompra;
	if(mtocompra > 1000)
	descuento = mtocompra * 0.20;	
	else
	descuento = 0;
	
	PagoTotal = mtocompra - descuento;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	Descuento();
	return 0;
}
```
</details>

##### Ejercicio 12. Calcular el total que una persona debe pagar en una librería, si se realiza una compra mayor a $5,000.00 se realizara un descuento del 5% además si la persona es estudiante se le otorgara un descuento extra del 3%
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_12
	Definir mtocompra, descuento, total_pago, est Como Entero
	mtocompra <- 0;
	descuento <- 0;
	total_pago <- 0;
	est <- 0;
	Escribir "------PROGRAMA QUE CALCULA EL TOTAL A PAGAR EN UNA LIBRERIA-----";
	Escribir "Ingrese el monto de la compra: ";
	Leer mtocompra;
	Escribir "¿Eres estudiante PRESIONA: 1)SI 2)NO?";
	Leer est;
	Si (mtocompra <= 5000 y est == 2) Entonces
		descuento <- 0;
	FinSi
	Si (mtocompra <= 5000 y est == 1) Entonces
		descuento <- mtocompra * 0.03;
	FinSi
	Si (mtocompra > 5000 y est == 2) Entonces
		descuento <- mtocompra * 0.05;
	FinSi
	Si (mtocompra > 5000 y est == 1) Entonces
		descuento <- mtocompra * 0.08;
	FinSi
	total_pago <- mtocompra - descuento;
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "Por el monto de la compra de",mtocompra," el total a pagar es de: $",total_pago;	
	Escribir "El descuento aplicado es de: $",descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int MtoCompra = 0, descuento = 0, TotalPago = 0, est = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"POR EL MONTO DE LA COMPRA DE "<<MtoCompra<<" EL TOTAL A PAGAR ES DE: $"<<TotalPago<<endl;
	cout<<"EL DESCUENTO APLICADO ES DE: $"<<descuento;
}
void Libreria()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR EN UNA LIBRERIA---"<<endl;
	cout<<"Ingrese el monto de la compra: $";
	cin>>MtoCompra;
	cout<<"Eres estudiante PRESIONA: 1)SI 2)NO: ";
	cin>>est;
	if(MtoCompra <= 5000 && est == 2)
	descuento = 0;
	if(MtoCompra <= 5000 && est == 1)
	descuento = MtoCompra * 0.03;
	if(MtoCompra > 5000 && est == 2)
	descuento = MtoCompra * 0.05;
	if(MtoCompra > 5000 && est == 1)
	descuento = MtoCompra * 0.08;
	
	TotalPago = MtoCompra - descuento;
	ImprimirDatos();
	
}
int main()
{
	system("color 0A");
	Libreria();
	return 0;
}
```
</details>

##### Ejercicio 13. Una tienda ofrece galletas a 10 pesos el kilo, pero comprando más de 100 kilos, se ofrece un 10 % de descuento. Hacer un programa que calcule el total a pagar
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_13
	Definir kilos, prckl, descuento, subtotal, monto_total Como Entero
	kilos <- 0;
	prckl <- 0;
	subtotal <- 0;
	descuento <- 0;
	monto_total <- 0;
	Escribir "----PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR X KILOS DE GALLETAS----";
	Escribir "Ingrese los kilos de galletas a comprar: ";
	Leer kilos;
	Escribir "Ingrese el precio por kilo de las galletas: ";
	Leer prckl;
	subtotal <- kilos * prckl;
	Si (kilos > 100) Entonces
		descuento <- kilos * 0.10;
	SiNo
		descuento <- 0;
	FinSi
	monto_total <- subtotal - descuento;
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El total a pagar por ",kilos," kilos de galletas es de: $",monto_total;
	Escribir "El descuento aplicado es de: $",descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int kilos = 0, prckl = 0, descuento = 0, subtotal = 0, MontoTotal = 0;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL TOTAL A PAGAR POR "<<kilos<<" KILOS DE GALLETAS ES DE: $"<<MontoTotal<<endl;
	cout<<"EL DESCUENTO APLICADO ES DE: $"<<descuento;
}
void KilosGalletas()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR X KILOS DE GALLETAS---"<<endl;
	cout<<"Ingrese los kilos de galletas a comprar: ";
	cin>>kilos;
	cout<<"Ingrese el precio por kilo de las galletas: $";
	cin>>prckl;
	subtotal = kilos * prckl;
	if(kilos > 100)
	descuento = kilos * 0.10;
	else
	descuento = 0;
	
	MontoTotal = subtotal - descuento;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	KilosGalletas();
	return 0;
}
```
</details>

##### Ejercicio 14. En una fábrica de calzado pagan 20 pesos por cada par empaquetado. Si se empaquetan más de 500 zapatos, los pares extras se pagan a 30 pesos. Hacer un programa que calcule el sueldo de un trabajador con base en el número de pares empaquetados
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_14
	Definir numzap, precio_empqtd, sueldo Como Entero
	numzap <- 0;
	precio_empqtd <- 0;
	sueldo <- 0;
	Escribir "------PROGRAMA QUE CALCULA EL SUELDO DE UN TRABAJADOR-----";
	Escribir "Ingrese la cantidad de zapatos empaquetados: ";
	Leer numzap;
	Escribir "Ingrese el precio de cada par empaquetado: ";
	Leer precio_empqtd;
	Si (numzap > 500) Entonces
		sueldo <- numzap * 30;
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El sueldo que persive por ",numzap," pares de calzado es de: $",sueldo;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void FabricaCalzado()
{
	int numzap = 0, PreEmpqtd = 0, sueldo = 0;
	cout<<"\t---PROGRAMA QUE CALCULA EL SUELDO DE UN TRABAJADOR---"<<endl;
	cout<<"Ingrese la cantidad de zapatos empaquetados: ";
	cin>>numzap;
	cout<<"Ingrese el precio de cada par empaquetado: $";
	cin>>PreEmpqtd;
	system("cls");
	if(numzap > 500)
	sueldo = numzap * 30;
	
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL SUELDO QUE PERSIVE POR "<<numzap<<" PARES DE CALZADO ES DE: $"<<sueldo;
}
int main()
{
	system("color 0A");
	FabricaCalzado();
	return 0;
}
```
</details>

##### Ejercicio 15. Un maestro desea evaluar dando equivalencia con letras, de 8.5 a 10 equivale a MB, de 7 a 8.4 equivale a B, de 6 a 6.9 equivale a S, de 0 a 5.9 equivale a NA. Crear un programa que realice la equivalencia
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_15
	Definir calif Como Real
	Definir equiv Como Caracter
	calif <- 0;
	Escribir "----PROGRAMA QUE CONVIERTA LA CALIFICACION DE NUMERO A LETRA----";
	Escribir "Ingrese su calificación: ";
	Leer calif;
	Si (calif >= 8.5 y calif <= 10) Entonces
		equiv <- "MB";
	SiNo
		Si (calif >= 7 y calif <= 8.4) Entonces
			equiv <- "B";
		SiNo
			Si (calif >= 6 y calif <= 6.9) Entonces
				equiv <- "S";
			SiNo
				Si (calif >= 0 y calif <= 5.9) Entonces
					equiv <- "N/A";
				FinSi
			FinSi
		FinSi
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "La calificación de ",calif," es equivalente a: ",equiv;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
float calif = 0;
string equiv;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"LA CALIFICACION DE "<<calif<<" ES EQUIVALENTE A: "<<equiv;
}
void EquivCalif()
{
	cout<<"\t---PROGRAMA QUE CONVIERTA LA CALIFICACION DE NUMERO A LETRA---"<<endl;
	cout<<"Ingrese su calificacion: ";
	cin>>calif;
	if (calif >= 8.5 && calif <= 10)
	equiv = "MB";
	if (calif >= 7 && calif <= 8.4)
	equiv = "B";
	if (calif >= 6 && calif <= 6.9)
    equiv = "S";
	if (calif >= 0 && calif <= 5.9)
	equiv = "N/A";
	ImprimirDatos();
}
int main ()
{
	system("color 0A");
	EquivCalif();
	return 0;
}
```
</details>

##### Ejercicio 16. Determinar la cantidad semanal de dinero que recibirá cada uno de los obreros de una empresa. Se sabe que cuando las horas que trabajo un obrero exceden de 40, el resto se convierte en horas extras que se pagan al doble de una hora normal, cuando no exceden de 8; cuando las horas extras exceden de 8 se pagan las primeras 8 al doble de lo que se paga por una hora normal y el resto al triple
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_16
	Definir hrstrab, hrsextras, hrstriple Como Entero
	Definir pagohrs, sueldo Como Real
	hrstrab <- 0;
	hrsextras <- 0;
	hrstriple <- 0;
	pagohrs <- 0;
	sueldo <- 0;
	Escribir "------PROGRAMA QUE CALCULA LA CANTIDAD SEMANAL DE DINERO------";
	Escribir "Ingrese sus horas trabajadas: ";
	Leer hrstrab;
	Escribir "Ingrese el pago por hora: ";
	Leer pagohrs;
	Si (hrstrab > 40) Entonces
		hrsextras <- hrstrab - 40;
		Si (hrsextras > 8) Entonces
			hrstriple <- hrsextras - 8;
			sueldo <- (40 * pagohrs) + (8 * pagohrs * 2) + (hrstriple * pagohrs * 3);
		SiNo
			sueldo <- (40 * pagohrs) + (hrsextras * pagohrs * 2);
		FinSi
	SiNo
		sueldo <- hrstrab * pagohrs;
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "La cantidad semanal de dinero a recibir por ",hrstrab," horas trabajadas es de: $",sueldo; 
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void SalarioObrero()
{
	int hrstrab = 0, hrsextras = 0, hrstriple = 0;
	float pagohrs = 0, sueldo = 0;
	cout<<"\t---PROGRAMA QUE CALCULA LA CANTIDAD SEMANAL DE DINERO---"<<endl;
	cout<<"Ingrese sus horas trabajadas a la semana: ";
	cin>>hrstrab;
	cout<<"Ingrese el pago por hora: $";
	cin>>pagohrs;
	system("cls");
	if(hrstrab > 40)
	{
		hrsextras = hrstrab - 40;
		if(hrsextras > 8)
		{
			hrstriple = hrsextras - 8;
		    sueldo = (40 * pagohrs) + (8 * pagohrs * 2) + (hrstriple * pagohrs * 3);
		}
		else
		sueldo = (40 * pagohrs) + (hrsextras * pagohrs * 2);
	}
	else
	sueldo = hrstrab * pagohrs;
	
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"LA CANTIDAD SEMANAL DE DINERO A RECIBIR POR "<<hrstrab<<" HORAS TRABAJADAS ES DE: $"<<sueldo;
}
int main()
{
	system("color 0A");
	SalarioObrero();
	return 0;
}
```
</details>

##### Ejercicio 17. En una fábrica de computadoras se planea ofrecer a los clientes un descuento que dependerá del número de computadoras que compre. Si las computadoras son menos de cinco se les dará un 10% de descuento sobre el total de la compra; si el número de computadoras es mayor o igual a cinco, pero menos de diez se le otorga un 20% de descuento; y si son 10 o más se les da un 40% de descuento
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_17
	Definir numcompu, preccompu, descuento, total_compra, subtotal Como Real
	numcompu <- 0;
	preccompu <- 0;
	descuento <- 0;
	total_compra <- 0;
	subtotal <- 0;
	Escribir "----PROGRAMA QUE CALCULA EL DESCUENTO DE UNA FABRICA DE COMPUTADORAS----";
	Escribir "Ingrese el numero de computadoras a comprar: ";
	Leer numcompu;
	Escribir "Ingrese el precio de la computadora: ";
	Leer preccompu;
	subtotal <- numcompu * preccompu;
	Si (numcompu < 5) Entonces
		descuento <- subtotal * 0.10;
	SiNo
		Si (numcompu >= 5 y numcompu < 10) Entonces
			descuento <- subtotal * 0.20;
		SiNo
			Si (numcompu >= 10) Entonces
				descuento <- subtotal * 0.40;
			FinSi
		FinSi
	FinSi
	total_compra <- subtotal - descuento;
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El total a pagar por ",numcompu," computadoras compradas es de: $",total_compra;
	Escribir "El descuento aplicado es de: $",descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
int numPC = 0, precPC = 0, descuento = 0, TotalCompra = 0, subtotal = 0;
void FabricaPC()
{
	cout<<"\t---PROGRAMA QUE CALCULA EL DESCUENTO DE UNA FABRICA DE COMPUTADORAS---"<<endl;
	cout<<"Ingrese el numero de computadoras a comprar: ";
	cin>>numPC;
	cout<<"Ingrese el precio de la computadora: $";
	cin>>precPC;
	subtotal = numPC * precPC;
	system("cls");
	if(numPC < 5)
	descuento = subtotal * 0.10;
	if(numPC >= 5 && numPC < 10)
	descuento = subtotal * 0.20;
	if(numPC >= 10)
	descuento = subtotal * 0.40;
	
	TotalCompra = subtotal - descuento;
	
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL TOTAL A PAGAR POR "<<numPC<<" COMPUTADORAS COMPRADAS ES DE: $"<<TotalCompra<<endl;
    cout<<"EL DESCUENTO APLICADO ES DE: $"<<descuento;
}
int main()
{
	system("color 0A");
	FabricaPC();
	return 0;
}
```
</details>

##### Ejercicio 18. En un juego de preguntas a las que se responde “Si” o “No” gana quien responda correctamente las tres preguntas. Si se responde mal a cualquiera de ellas ya no se pregunta la siguiente y termina el juego. Las preguntas son:
- ¿Colon descubrió América?
- ¿La independencia de México fue en el año 1810?
- ¿The Doors fue un grupo de rock americano?
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_18
	Definir respuesta Como Caracter
	Escribir "------BIENVENIDO AL JUEGO DE PREGUNTAS SOBRE CULTURA GENERAL------";
	Escribir "¿Colón descubrió América? ";
	Leer respuesta;
	Si (respuesta == "SI") Entonces
		Escribir "¿La independencia de México fue en el año 1810? ";
		Leer respuesta;
		Si (respuesta == "SI") Entonces 
			Escribir "¿The Doors fue un grupo de rock americano? ";
			Leer respuesta;
			Si (respuesta == "SI") Entonces 
				Escribir "!!!FELICIDADES HAS GANADO!!!..... !!!SIGUE ASI!!! ";
			SiNo
				Escribir "LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!";
			FinSi
		SiNo
			Escribir "LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!";
		FinSi
	SiNo
		Escribir "LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!";
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void JuegoPreguntas()
{
	string respuesta;
	cout<<"\t---BIENVENIDO AL JUEGO DE PREGUNTAS SOBRE CULTURA GENERAL---"<<endl;
	cout<<"1.-¿Colon descubrio America?"<<endl;
	cin>>respuesta;
	if(respuesta == "si" || respuesta == "SI")
	{
		cout<<"2.-¿La independencia de Mexico fue en 1810?"<<endl;
		cin>>respuesta;
		if(respuesta == "si" || respuesta == "SI")
		{
			cout<<"3.-¿The Doors fue un grupo de rock americano?"<<endl;
	        cin>>respuesta;
	        if(respuesta == "si" || respuesta == "SI")
	        cout<<"!!!FELICIDADES HAS GANADO!!!..... !!!SIGUE ASI!!! "<<endl;
	        else
	        cout<<"LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!! "<<endl;
		}
		else
		cout<<"LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!! "<<endl;	    
	}
	else
	cout<<"LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!! "<<endl;	
}
int main()
{
	system("color 0A");
	JuegoPreguntas();
	return 0;
}
```
</details>

<details>
<summary>Python</summary>

```Python
def juego_preguntas():
    print("\t---BIENVENIDO AL JUEGO DE PREGUNTAS SOBRE CULTURA GENERAL---")

    respuesta = input("1.-¿Colon descubrio America? ")

    if respuesta.lower() == "si":
        respuesta = input("2.-¿La independencia de Mexico fue en 1810? ")

        if respuesta.lower() == "si":
            respuesta = input("3.-¿The Doors fue un grupo de rock americano? ")

            if respuesta.lower() == "si":
                print("!!!FELICIDADES HAS GANADO!!!..... !!!SIGUE ASI!!!")
            else:
                print("LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!")
        else:
            print("LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!")
    else:
        print("LO SENTIMOS.....!!!HAS PERDIDO!!!.....!!!SUERTE PARA LA PROXIMA!!!")

# Ejecutar juego
juego_preguntas()
```
</details>

##### Ejercicio 19. Un proveedor de estéreos ofrece un descuento del 10% sobre el precio sin IVA, de algún aparato si esta cuesta $2000 o más. Además, independientemente de esto, ofrece un 5% de descuento si la marca es “sony”. Determinar cuánto pagara, con IVA incluido, un cliente cualquiera por la compra de su aparato
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_19
	Definir precio,total,descuento,iva, porcentaje, marca Como Real
	precio <- 0;
	total <- 0;
	descuento <- 0;
	iva <- 0;
	porcentaje <- 0;
	marca <- 0;
	Escribir "------PROGRAMA QUE CALCULA CUANTO PAGARA UNA PERSONA POR UN ESTEREO-----";
	Escribir "Ingresa el precio del aparato: ";
	leer precio;
	Escribir "¿La marca es SONY?: PRESIONA 1)SI 2)NO";
	leer marca;
	total <- precio;
	Escribir "Ingresa el porcentaje de IVA aplicar: ";
	leer porcentaje;
	Si marca == 1 y precio >= 2000  Entonces 
		descuento = precio * 0.15;
	SiNo
		Si precio >= 2000 Entonces
			descuento = precio * 0.10;
		FinSi
	FinSi
	total <- precio - descuento;
	iva <- (total * porcentaje) / 100;
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El total a pagar es: $",total;
	Escribir "El descuento aplicado es: $",descuento;
	Escribir "El IVA aplicado es: $",iva;
	Escribir "El total a pagar con el IVA incluido es: $",total + iva;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
float precio = 0, total = 0, descuento = 0, porcentaje = 0, iva = 0;
string marca;
void ImprimirDatos()
{
	system("cls");
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"DESCUENTO APLICADO: "<<descuento<<endl;
	cout<<"IVA APLICADO: $"<<iva<<endl;
	cout<<"TOTAL A PAGAR CON EL IVA INCLUIDO: $"<<total + iva<<endl;
}
void ProveedorEstereos()
{
	cout<<"\t---PROGRAMA QUE CALCULA CUANTO PAGARA UNA PERSONA POR UN ESTEREO---"<<endl;
	cout<<"Ingresa el precio del estereo: $";
	cin>>precio;
	cout<<"Ingresa la marca del estereo: ";
	cin>>marca;
	total = precio;
	cout<<"Ingresa el porcentaje de IVA aplicar: ";
	cin>>porcentaje;
	if(marca == "SONY" && precio >= 2000)
	descuento = precio * 0.5;
	else
	{
		if(precio >= 2000)
		descuento = precio * 0.10;
	}
	total = precio - descuento;
	iva = (total * porcentaje) / 100;
	ImprimirDatos();
}
int main()
{
	system("color 0A");
	ProveedorEstereos();
	return 0;
}
```
</details>

##### Ejercicio 20. Una frutería ofrece las manzanas con descuento según la siguiente tabla:
| NUM. DE KILOS COMPRADOS    |    % DESCUENTO    |
| :---:                      |     :--:          |
|        0 - 2               |       0%          | 
|      2.01 - 5              |      10%          | 
|      5.01 - 10             |      15%          | 
|  10.01 en adelante         |      20%          | 
##### Determinar cuánto pagara una persona que compre manzanas es esa frutería
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_20
	Definir kilo Como Entero
	Definir precio,total,descuento Como Real
	kilo <- 0;
	precio <- 0;
	total <- 0;
	descuento <- 0;
	Escribir "------PROGRAMA QUE CALCULA EL TOTAL DE LA COMPRA POR MANZANAS------";
	Escribir "Ingrese los kilos de manzanas: ";
	leer kilo;
	Escribir "Ingrese el precio del kilo de manzanas";
	leer precio;
	total = precio * kilo;
	Si (kilo <= 2) Entonces
		descuento = 0;
	SiNo
		Si (kilo >= 2.01 y kilo <= 5) Entonces
			descuento = total * 0.10;
			Escribir "Se aplico un 10% de descuento";
		SiNo
			Si (kilo >= 5.01 y kilo <= 10) Entonces
				descuento = total * 0.15;
				Escribir "Se aplico un 15% de descuento";
			SiNo
				descuento = total * 0.20;
				Escribir "Se aplico un 20% de descuento";
			FinSi
		FinSi
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El descuento aplicado es: $",descuento;
	Escribir "El total a pagar por ",kilo," kilos de manzana es: $",total - descuento;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void Fruteria()
{
	int kilo = 0;
	float precio = 0, subtotal = 0, descuento = 0, TotalCompra = 0;
	cout<<"\t---PROGRAMA QUE CALCULA EL SUELDO DE UN TRABAJADOR---"<<endl;
	cout<<"Ingrese los kilos de manzanas: ";
	cin>>kilo;
	cout<<"Ingrese el precio del kilo de manzanas: $";
	cin>>precio;
	subtotal = precio * kilo;
	system("cls");
	if(kilo <= 2)
	descuento = 0;
	if(kilo >= 2.01 && kilo <= 5)
	{
		descuento = subtotal * 0.10;
		cout<<"SE APLICO UN DESCUENTO DEL 10%\n"<<endl;
	}
	if(kilo >= 5.01 && kilo <= 10)
	{
		descuento = subtotal * 0.15;
		cout<<"SE APLICO UN DESCUENTO DEL 15%\n"<<endl;
	}
	else
	{
		descuento = subtotal * 0.20;
		cout<<"SE APLICO UN DESCUENTO DEL 20%\n"<<endl;
	}
	
	TotalCompra = subtotal - descuento;
	
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL DESCUENTO APLICADO ES DE: $"<<descuento<<endl;
	cout<<"EL TOTAL A PAGAR POR "<<kilo<<" KILOS DE MANZANAS ES DE: $"<<TotalCompra<<endl;
}
int main()
{
	system("color 0A");
	Fruteria();
	return 0;
}
```
</details>

##### Ejercicio 21. Una fábrica de sillas vende al público en general al mayoreo con un precio de $200 y menudeo con un precio de $300 por silla, para que un cliente obtenga el precio de mayoreo debe comprar más de 10 sillas, calcular el total a pagar por la compra de sillas
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_21
	Definir numslls, total_compra Como Entero
	numslls <- 0;
	total_compra <- 0;
	Escribir "----PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR LA COMPRA DE SILLAS----";
	Escribir "Ingrese la cantidad de sillas que desea llevar: ";
	Leer numslls;
	Si (numslls > 10) Entonces
		total_compra <- numslls * 200;
	SiNo
		total_compra <- numslls * 300;
	FinSi
	Escribir "------RESULTADOS OBTENIDOS------";
	Escribir "El total a pagar por la cantidad de ",numslls," sillas compradas es de: $",total_compra;
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void FabricaSillas()
{
	int numslls = 0, TotalCompra = 0;
	cout<<"\t---PROGRAMA QUE CALCULA EL TOTAL A PAGAR POR LA COMPRA DE SILLAS---"<<endl;
	cout<<"Ingrese la cantidad de sillas que desea llevar: ";
	cin>>numslls;
	system("cls");
	if(numslls > 10)
	TotalCompra = numslls * 200;
	else
	TotalCompra = numslls * 300;
	cout<<"\t---RESULTADOS OBTENIDOS---"<<endl;
	cout<<"EL TOTAL A PAGAR POR LA CANTIDAD DE "<<numslls<<" SILLAS COMPRADAS ES DE: $"<<TotalCompra;
}
int main()
{
	system("color 0A");
	FabricaSillas();
	return 0;
}
```
</details>

##### Ejercicio 22. Una escuela ofrece una beca a los alumnos cuyo promedio sea mayor o igual 9.0 y curse el primer o segundo año, desarrollar un algoritmo que muestre si los alumnos obtienen o no la beca estudiantil
<details>
<summary>Pseudocódigo</summary>

```
Algoritmo EJERCICIO_22
	Definir promedio,grado Como Entero
	promedio <- 0;
	grado <- 0;
	
	Escribir "------PROGRAMA QUE CALCULA SI UN ALUMNO TIENE DERECHO A UNA BECA------";
	Escribir "Ingrese su promedio: ";
	Leer promedio;
	Escribir "¿Eres estudiante de primero o segundo año?: PRESIONA 1)SI 2)NO";
	Leer grado;
	
	Si (promedio >= 9 y grado == 1) Entonces
		Escribir "Tu promedio ingresado de ",promedio," es ACEPTADO para una beca";
	SiNo
		Escribir "Tu promedio ingresado de ",promedio," es RECHAZADO para una beca";
	FinSi
FinAlgoritmo
```
</details>

<details>
<summary>C++</summary>

```c++
#include<iostream>
using namespace std;
void DerechoBeca()
{
	float promedio = 0;
	int grado = 0;
	cout<<"\t---PROGRAMA QUE CALCULA SI UN ALUMNO TIENE DERECHO A UNA BECA---"<<endl;
	cout<<"Ingrese su promedio: ";
	cin>>promedio;
	cout<<"Eres estudiante de primero o segundo grado: PRESIONA 1)SI 2)NO: ";
	cin>>grado;
	system("cls");
	if(promedio >= 9 && grado == 1)
	cout<<"TU PROMEDIO INGRESADO DE "<<promedio<<" ES ACEPTADO PARA LA BECA";
	else
	cout<<"TU PROMEDIO INGRESADO DE "<<promedio<<" ES RECHAZADO PARA LA BECA";	
}
int main()
{
	system("color 0A");
	DerechoBeca();
	return 0;
}
```
</details>