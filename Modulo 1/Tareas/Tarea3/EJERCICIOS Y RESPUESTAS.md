### Base de datos utilizada: 
<img width="479" height="151" alt="image" src="https://github.com/user-attachments/assets/98cc58a6-7ab9-445e-b0f2-10a54c9a2fca" />

# INSERT
## Tarea A:
1. Insertar un nuevo registro de instructor con id 4 para Sandip Saha que vive en Edmonton, CA en la tabla “Instructor”
```
INSERT INTO Instructor
  (ins_id, lastname, firstname, city, country)
VALUES
  (4, 'Saha', 'Sandip', 'Edmonton', 'CA');
```
2. Insertar dos nuevos registros de instructor en la tabla “Instructor”. Primer registro con id 5 para John Doe que vive en Sydney, AU. Segundo registro con id 6 para Jane Doe que vive en Dhaka, BD.
```
INSERT INTO Instructor
  (ins_id, lastname, firstname, city, country)
VALUES
  (5, 'Doe', 'John', 'Sydney', 'AU'),
  (6, 'Doe', 'Jane', 'Dhaka', 'BD')
```

## Tarea B:
1. Inserta un nuevo registro de instructor con id 7 para Antonio Cangiano que vive en Vancouver, CA en la tabla “Instructor”.
```
INSERT INTO Instructor
  (ins_id, lastname, firstname, city, country)
VALUES
  (7, 'Cangiano', 'Antonio', 'Vancouver', 'CA')
```

2. Inserta dos nuevos registros de instructor en la tabla “Instructor”. Primer registro con id 8 para Steve Ryan que vive en Barlby, GB. Segundo registro con id 9 para Ramesh Sannareddy que vive en Hyderabad, IN.
```
INSERT INTO Instructor
  (ins_id, lastname, firstname, city, country)
VALUES
  (8, 'Ryan', 'Steve', 'Barlby', 'GB'),
  (9, 'Sannareddy', 'Ramesh', 'Hyderabad', 'IN')
```

# UPDATE
## Tarea A:
1. Actualizar la ciudad de Sandip a Toronto.
```
UPDATE Instructor
SET City = 'Toronto'
WHERE firstname = 'Sandip'
```

2. Actualizar la ciudad y el país de Doe con id 5 a Dubái y AE respectivamente.
```
UPDATE Instructor
SET City = 'Dubái', Country = 'AE'
WHERE ins_id = 5
```

## Tarea B:
1. Actualiza la ciudad del registro del instructor a Markham cuyo id es 1.
```
UPDATE Instructor
SET City = 'Markham'
WHERE ins_id = 1
```

2. Actualiza la ciudad y el país de Sandip con id 4 a Dhaka y BD respectivamente.
````
UPDATE Instructor
SET City = 'Dhaka', Country = 'BD'
WHERE ins_id = 4
````

# DELETE
## Tarea A:
1. Eliminar el registro del instructor Doe cuyo id es 6.
````
DELETE FROM Instructor
WHERE ins_id = 6
````
2. Elimina el registro del instructor Hima.
````
DELETE FROM Instructor
WHERE firstname = 'Hima'
````











