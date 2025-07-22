DROP TABLE staff; 

CREATE TABLE staff ( 
id NUMBER PRIMARY KEY, 
name VARCHAR2(100), 
department VARCHAR2(50) 
); 

INSERT INTO staff (id, name, department) VALUES (1, 'Mathi', 'HR'); 
INSERT INTO staff (id, name, department) VALUES (2, 'Durga', 'IT');
INSERT INTO staff (id, name, department) VALUES (3, 'Suji', 'Team Lead');
INSERT INTO staff (id, name, department) VALUES (4, 'Priya', 'Finance'); 

UPDATE staff SET department = 'Software' WHERE id = 2; 
INSERT INTO staff (id, name, department) VALUES (5, 'John', 'Marketing'); 
ALTER TABLE staff ADD salary NUMBER(10,2);
UPDATE staff SET salary = 55000 WHERE id = 1; 
UPDATE staff SET salary = 60000 WHERE id = 2; 
UPDATE staff SET salary = 50000 WHERE id = 3;

COLUMN id FORMAT 999 HEADING 'ID' 
COLUMN name FORMAT A15 HEADING 'NAME'
COLUMN department FORMAT A20 HEADING 'DEPARTMENT' 
COLUMN salary FORMAT 999999 HEADING 'SALARY' 

SELECT * FROM staff; 
ALTER TABLE staff RENAME COLUMN department TO role; 
UPDATE staff 
SET name = 'Pugal' 
WHERE name = 'John';









