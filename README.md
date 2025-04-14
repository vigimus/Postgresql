# Postgresql kommandon:
 SELECT * FROM login;
  SELECT * FROM users;
  # SELECT COUNT(name) FROM  users;
  SELECT SUM(age) FROM  users;
  SELECT AVG(score) FROM  users;
   \d
SELECT * FROM users ORDER BY score ASC;
SELECT * FROM users ORDER BY score DESC;
SELECT * FROM users WHERE name LIKE 'V%';
UPDATE users SET score = 100 WHERE name='John' OR name='Sally'; 
 ALTER TABLE users ADD score smallint; 
 INSERT INTO users (name, age, birthday) VALUES ('John', 45, '1935-01-04'); 
 SELECT name, age, birthday FROM users;
CREATE TABLE users (name text, age smallint, birthday date);
SELECT * FROM users JOIN login ON users.name = login.name;
 DELETE FROM users WHERE name='John';
 DROP TABLE users;
 DROP TABLE login;
