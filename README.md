# Ds-Py-qstn

Q1)
A)
  SELECT DISTINCT name,imbd_score,premiered_on
  FROM movies
  WHERE premiered_on >= 2020-04-01;
  
 B)
   SELECT COUNT(genres.name)
   FROM genres INNER JOIN movies ON movies.genre_id=genres.id
   WHERE  premiered_on >=2000-01-01;
 C)SELECT name,COUNT(name) 
   FROM movies
   GROUPBY name
   HAVING COUNT(name)>1;
