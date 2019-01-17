# JDBC_Assignment1

SQL kod

CREATE DATABASE sqlandjava;

CREATE TABLE sqlandjava.people (
person_id INT NOT NULL AUTO_INCREMENT,
firstname VARCHAR(45),
lastname VARCHAR(45),
PRIMARY KEY(person_id));
INSERT INTO sqlandjava.people (person_id, firstname, lastname)
VALUES (1, 'Anna', 'Bolt'),
(2, 'Carl', 'Dolk'),
(3, 'Erik', 'Fram'),
(4, 'Gina', 'Hult');

SELECT * FROM sqlandjava.people;

CREATE USER karin@localhost IDENTIFIED BY 'sorlin';
GRANT SELECT ON sqlandjava.people TO karin@localhost;
