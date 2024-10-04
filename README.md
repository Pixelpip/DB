## SQL QUERIES

```
SHOW DATABASES;
use students;

CREATE TABLE students (
    usn VARCHAR(15) PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    pincode VARCHAR(10),
    dob DATE
);

ALTER TABLE students
ADD phone_number VARCHAR(15);



INSERT INTO students (usn, name, email, pincode, dob, phone_number) VALUES
('4MW22CS001', 'ABEY', 'ABEY@COLLEGE.com', '123456', '2000-01-01', '1234567890'),
('4MW22CS002', 'ABHILASH', 'ABHILASH@COLLEGE.com', '654321', '2000-02-02', '0987654321');

UPDATE students
SET email = 'new@NEW,COM'
WHERE usn = '4MW22CS001';

SELECT * FROM students;




```