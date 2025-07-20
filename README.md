# ManyMeal ;

CREATE TABLE DEPOSIT (
    ACTNO INT,
    CNAME VARCHAR(50),
    BNAME VARCHAR(50),
    AMOUNT DECIMAL(8,2),
    ADATE DATETIME
);

CREATE TABLE BRANCH (
    BNAME VARCHAR(50),
    CITY VARCHAR(50)
);

CREATE TABLE CUSTOMERS (
    CNAME VARCHAR(50),
    CITY VARCHAR(50)
);
CREATE TABLE BORROW (
    LOANNO INT,
    CNAME VARCHAR(50),
    BNAME VARCHAR(50),
    AMOUNT DECIMAL(8,2)
);


INSERT INTO DEPOSIT (ACTNO, CNAME, BNAME, AMOUNT, ADATE) VALUES
(101, 'ANIL', 'VRCE', 1000.00, '1995-03-01'),
(102, 'SUNIL', 'AJNI', 5000.00, '1996-04-01'),
(103, 'MEHUL', 'KAROLBAGH', 3500.00, '1995-11-17'),
(104, 'MADHURI', 'CHANDI', 1200.00, '1995-12-17'),
(105, 'PRAMOD', 'M.G. ROAD', 3000.00, '1996-03-27'),
(106, 'SANDIP', 'ANDHERI', 2000.00, '1996-01-31'),
(107, 'SHIVANI', 'VIRAR', 1000.00, '1995-05-09'),
(108, 'KRANTI', 'NEHRU PLACE', 5000.00, '1995-07-02'),
(109, 'MINU', 'POWAI', 7000.00, '1995-10-08');


INSERT INTO BRANCH (BNAME, CITY) VALUES
('VRCE', 'NAGPUR'),
('AJNI', 'NAGPUR'),
('KAROLBAGH', 'DELHI'),
('CHANDI', 'DELHI'),
('DHARAMPETH', 'NAGPUR'),
('M.G. ROAD', 'BANGLORE'),
('ANDHERI', 'BOMBAY'),
('VIRAR', 'BOMBAY'),
('NEHRU PLACE', 'DELHI'),
('POWAI', 'BOMBAY');


INSERT INTO BORROW (LOANNO, CNAME, BNAME, AMOUNT) VALUES
(201, 'ANIL', 'VRCE', 1000.00),
(206, 'MEHUL', 'AJNI', 5000.00),
(311, 'SUNIL', 'DHARAMPETH', 3000.00),
(321, 'MADHURI', 'ANDHERI', 2000.00),
(375, 'PRAMOD', 'VIRAR', 8000.00),
(481, 'KRANTI', 'NEHRU PLACE', 3000.00);


INSERT INTO CUSTOMERS (CNAME, CITY) VALUES
('ANIL', 'CALCUTTA'),
('SUNIL', 'DELHI'),
('MEHUL', 'BARODA'),
('MANDAR', 'PATNA'),
('MADHURI', 'NAGPUR'),
('PRAMOD', 'NAGPUR'),
('SANDIP', 'SURAT'),
('SHIVANI', 'BOMBAY'),
('KRANTI', 'BOMBAY'),
('NAREN', 'BOMBAY');



CREATE TABLE STUDENT (
    StuID INT PRIMARY KEY,
    FirstName VARCHAR(25),
    LastName VARCHAR(25),
    Website VARCHAR(50),
    City VARCHAR(25),
    Address VARCHAR(100)
);

INSERT INTO STUDENT (StuID, FirstName, LastName, Website, City, Address)
VALUES
(1011, 'Keyur', 'Patel', 'techonthenet.com', 'Rajkot', 'A-303 ‘Vasant Kunj’, Rajkot'),
(1022, 'Hardik', 'Shah', 'digminecraft.com', 'Ahmedabad', '“Ram Krupa”, Raiya Road'),
(1033, 'Kajal', 'Trivedi', 'bigactivities.com', 'Baroda', 'Raj bhavan plot, near garden'),
(1044, 'Bhoomi', 'Gajera', 'checkyourmath.com', 'Ahmedabad', '“Jig’s Home”, Narol'),
(1055, 'Harmit', 'Mitel', '@me.darshan.com', 'Rajkot', 'B-55, Raj Residency'),
(1066, 'Ashok', 'Jani', NULL, 'Baroda', 'A502, Club House Building');


