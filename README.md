Vamos a trabajar con nuestra primera base de datos de SQL. Crea una base de datos nueva llamada `building`:

### [](https://github.com/GammaTechSchool/MAD_PART_JsCao_1/blob/main/src/backend/exercises/sql1.md#ejercicio-1)Ejercicio 1

1.Crear tabla `aparments`
```sql
CREATE TABLE apartments(
apartment_id INTEGER PRIMARY KEY,
name STRING,
rooms INTEGER,
area NUMERIC
);
```
2. Tabla `families` 
```sql
CREATE TABLE families(
family_id INTEGER PRIMARY KEY,
name STRING,
members INTEGER,
aparment INTEGER,
);
```

### [](https://github.com/GammaTechSchool/MAD_PART_JsCao_1/blob/main/src/backend/exercises/sql1.md#ejercicio-2)Ejercicio 2

1. `apartments`
```sql
INSERT INTO apartments(apartment_id, rooms, area,name)
VALUES (5, 5, 55, 'los ciegos')
```

![alt text](https://i.imgur.com/tDxoP0j.png)

2. `families` 


```sql
INSERT INTO families(family_id, name, members,apartment)
VALUES (5,'Contreras', 1, 5)
```
![alt text](https://i.imgur.com/3wWZm5F.png)




### [](https://github.com/GammaTechSchool/MAD_PART_JsCao_1/blob/main/src/backend/exercises/sql1.md#ejercicio-3)Ejercicio 3

Realiza las siguientes consultas a la base de datos:

1. Obtén todas filas y columnas de la tabla `families`.
```sql
SELECT family_id, name, members, apartment                 
FROM families  
```
 ![alt text](https://i.imgur.com/3wWZm5F.png) 


2. Obtén los nombres de todas las familias de `families`.
```sql
SELECT name                
FROM families  
```
 ![alt text](https://i.imgur.com/F30r3NA.png) 


3. Obtén todos los pisos de la tabla `apartments` que tengan más de 2 habitaciones.

```sql
SELECT name
FROM apartments  
WHERE rooms > 2
```
 ![alt text](https://i.imgur.com/Q7tXj1T.png) 


4. Obtén todos los nombres de los pisos de la tabla `partaments` que tengan más de `100` metros cuadrados y más de `3` habitaciones.
```sql
SELECT name
FROM apartments  
WHERE rooms > 3 AND area > 99
```
 ![alt text](https://i.imgur.com/s2g3keD.png) 


5. Obtén el número de miembros de las familias que tengan más de `2` miembros, y ordena los resultados de menor a mayor.
```sql
SELECT name, members
FROM families  
WHERE members > 3 
ORDER BY members 
```
 ![alt text](https://i.imgur.com/xSjzFlw.png) 

6. Obtén el nombre de los apartamentos que tengan `2` o más baños, o `2` o más habitaciones.
```sql
SELECT name,bathrooms, rooms
FROM apartments
WHERE bathrooms > 2 OR rooms > 2
```
 ![alt text](https://i.imgur.com/DBtOrSK.png) 


7. Obtén los nombres de las familias que vivan en pisos de menos de `3` habitaciones.
```sql
fa
```
 ![alt text]() 



8. Obtén todas las columnas de las familias que vivan en pisos de más de `74` metros cuadrados.
```sql

```
 ![alt text]() 

9. Obtén el nombre de los pisos que tengan más de `2` inquilinos.
```sql

```
 ![alt text]() 

10. Obtén el nombre de los pisos que tengan menos de `3` inquilinos y más de `2` habitaciones.

```sql

```
 ![alt text]() 
