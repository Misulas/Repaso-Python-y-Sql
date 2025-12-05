# COUNT
### 1. Recupera el número de ubicaciones de las películas dirigidas por Woody Allen.
```
SELECT COUNT(Locations) FROM FilmLocations WHERE Director="Woody Allen";
```

### 2. Recupera el número de películas filmadas en Russian Hill.
```
SELECT COUNT(Title) from FilmLocations WHERE locations = "Russian Hill"

o su equivalente:
SELECT COUNT(*) from FilmLocations WHERE locations = "Russian Hill"
```

### 3. Recupera el número de filas que tienen un año de lanzamiento anterior a 1950 de la tabla "FilmLocations".
```
SELECT COUNT(Title) from FilmLocations WHERE ReleaseYear < 1950
```
# DISTINCT

### 1. Recupera los nombres de todas las películas únicas estrenadas en el siglo XXI y en adelante, junto con sus años de estreno.

```
SELECT DISTINCT Title, ReleaseYear from FilmLocations WHERE ReleaseYear >= 2000
```

### 2. Recupera los nombres de los directores y sus películas distintas filmadas en el City Hall.

```
SELECT DISTINCT Title, Director FROM FilmLocations WHERE Locations="City Hall";
```

# LIMIT

### 1. Recupera los nombres de las primeras 50 películas.

```
SELECT DISTINCT Title FROM FilmLocations LIMIT 50;
```

### 2. Recupera los primeros 10 nombres de películas estrenadas en 2015.

```
SELECT Title from FilmLocations WHERE ReleaseYear = 2015 LIMIT 10
```

### 3. Recupera los siguientes 3 nombres de películas que siguen después de las primeras 5 películas estrenadas en 2015.

```
SELECT DISTINCT TItle FROM FilmLocations where ReleaseYear = 2015 LIMIT 3 offset 5
```
