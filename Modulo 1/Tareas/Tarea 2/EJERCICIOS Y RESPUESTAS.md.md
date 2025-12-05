
### 1. Recupera los datos curiosos y las locaciones de filmación de todas las películas.
```
SELECT FunFacts, Locations FROM FilmLocations
```

### 2. Recupera los nombres de todas las películas estrenadas en el siglo XX y antes (años de estreno antes de 2000, incluyendo 2000), junto con las ubicaciones de filmación y los años de estreno.
```
SELECT Title, Locations, ReleaseYear FROM FilmLocations WHERE ReleaseYear <= 2000.
```

### 3. Recupera los nombres, nombres de las compañías productoras, ubicaciones de filmación y años de estreno de las películas que no fueron escritas por James Cameron.
```
SELECT Title, ProductionCompany, Locations, ReleaseYear FROM FilmLocations WHERE Writer <> "James Cameron"
```
