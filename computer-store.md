<h1 align="center">
EJERCICIOS DE BASE DE DATOS<br>
(TIENDA INFORMÁTICA)
</h1>

---

##### CREAR LA BASE DE DATOS
<details>
<summary>Solución</summary>

```sql
CREATE DATABASE tienda_informatica;
```
</details>

##### MOSTRAR LA BASE DE DATOS
<details>
<summary>Solución</summary>

```sql
SHOW DATABASE;
```
</details>

##### USAR LA BASE DE DATOS
<details>
<summary>Solución</summary>

```sql
USE tienda_informatica;
```
</details>

##### CREAR LA TABLA Y SUS CAMPOS
<details>
<summary>Solución</summary>

```sql
CREATE TABLE fabricante (
    fabricante_id INT AUTO_INCREMENT  NOT NULL,
    nombre VARCHAR(30)                NOT NULL,
    PRIMARY KEY (fabricante_id)
)ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

CREATE TABLE articulo (
    articulo_id INT AUTO_INCREMENT  NOT NULL,
    nombre VARCHAR(30)              NOT NULL,
    precio DECIMAL(10,2)            NOT NULL,
    PRIMARY KEY (articulo_id)
    CONSTRAINT fk_articulo_fabricante
        FOREIGN KEY (fabricante_id) REFERENCES fabricante(fabricante_id)
)ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
```
</details>


##### MOSTRAR LAS TABLAS
<details>
<summary>Solución</summary>

```sql
SHOW TABLES;
```
</details>


##### MOSTRAR LAS CARACTERÍSTICAS DE LA TABLA
<details>
<summary>Solución</summary>

```sql
DESCRIBE fabricante;
DESCRIBE articulo;
```
</details>

##### INSERCIÓN DE REGISTROS
<details>
<summary>Solución</summary>

```sql

```
</details>

---

<h1 align="center">CONSULTAS</h1>

##### Ejercicio 1. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 2. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 3. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 4. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 5. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 6. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 7. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 8. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 9. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 10. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 11. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 12. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 13. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 14. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 15. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 16. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 17. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 18. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 19. 
<details>
<summary>Solución</summary>

```sql

```
</details>

##### Ejercicio 20. 
<details>
<summary>Solución</summary>

```sql

```
</details>