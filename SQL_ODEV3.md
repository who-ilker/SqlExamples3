1)SELECT * FROM country
  WHERE country LIKE 'A%a';

2)SELECT * FROM country
  WHERE length(country) >= 6 AND country LIKE '%n';

3)SELECT * FROM film
 WHERE LENGTH(REPLACE (LOWER(title), 't','') ) <= LENGTH(title) - 4;

4)SELECT * FROM film 
  WHERE title LIKE 'C%' 
  AND LENGTH(title) > 90 
  AND rental_rate = 2.99;