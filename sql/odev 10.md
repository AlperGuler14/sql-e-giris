# SQL Homework 10

## 1.city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.

```sql
SELECT country,city FROM country 
LEFT JOIN city ON city.country_id = country.country_id;
```

## 2.customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

```sql
SELECT payment_id, first_name ,last_name FROM customer
RIGHT JOIN payment ON payment.customer_id =customer.customer_id;
```


## 3.customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.

```sql
SELECT rental_id , first_name ,last_name FROM rental
FULL JOIN customer ON customer.customer_id =rental.customer_id;
```
