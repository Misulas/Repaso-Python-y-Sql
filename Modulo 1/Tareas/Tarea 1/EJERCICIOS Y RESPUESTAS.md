### 1. Recupera los datos curiosos y las locaciones de filmación de todas las películas.
```
SELECT FunFacts, Locations FROM FilmLocations
```

2. Recupera los nombres de todas las películas estrenadas en el siglo XX y antes (años de estreno antes de 2000, incluyendo 2000), junto con las ubicaciones de filmación y los años de estreno.
```
SELECT Title, Locations, ReleaseYear FROM FilmLocations WHERE ReleaseYear <= 2000.
```
