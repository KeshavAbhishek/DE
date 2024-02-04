# EXPERIMENT 1 (DATABASE ENGINEERING)

* CREATE TABLE R2201020582_DETAILS(NAME VARCHAR(10) NOT NULL, PATIENT_ID NUMBER(5,0) PRIMARY KEY, DISEASE VARCHAR(15) NOT NULL, GENDER VARCHAR(3) NOT NULL, TREATMENT_PERIOD VARCHAR(10) NOT NULL);
* DESC R2201020582_DETAILS;
![Alt text](<IMAGES/Screenshot 2024-01-25 194849.png>)

* ALTER TABLE R2201020582_DETAILS ADD (AGE NUMBER(3,0) NOT NULL, ADMISSION_DATE DATE NOT NULL);
* DESC R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 195551.png>)

* ALTER TABLE R2201020582_DETAILS RENAME COLUMN ADMISSION_DATE TO ADMIT_DATE;
* DESC R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 200826.png>)

* ALTER TABLE R2201020582_DETAILS DROP(AGE, ADMIT_DATE);
* DESC R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 201848.png>)

* ALTER TABLE R2201020582_DETAILS ADD (DISCHARGE_DATE DATE NOT NULL);
* DESC R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 204028.png>)

* INSERT INTO R2201020582_DETAILS VALUES('Ram',101,'Commom_cold','M','3days','2-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Hari',102,'Cancer','M','56days','4-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Priya',103,'COVID-19','F','84days','6-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Rohit',104,'COVID-19','M','50days','8-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Priti',105,'Flu','F','5days','10-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Laxman',106,'Cancer','M','56days','12-10-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Hari',107,'Cancer','M','56days','10-14-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Sita',108,'Stomach_Aches','F','10days','10-16-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Priya',109,'Allergies','F','2days','10-18-1890');
* INSERT INTO R2201020582_DETAILS VALUES('Bharat',119,'Cold&flu','M','1day','10-20-1890');
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 205118.png>)

* INSERT INTO R2201020582_DETAILS VALUES('RAJAT',110,'Cold','M','3days','2/22/2012');
* INSERT INTO R2201020582_DETAILS VALUES('KAJAL',111,'Flu','F','4days','12/03/1999');
* INSERT INTO R2201020582_DETAILS VALUES('BISWAL',112,'Cancer','M','4days','05/02/2012');
![Image](<IMAGES/Screenshot 2024-01-25 212531.png>)

* UPDATE R2201020582_DETAILS SET PATIENT_ID = 44 WHERE PATIENT_ID=104;
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 212821.png>)

* UPDATE R2201020582_DETAILS SET NAME = 'ROHIT' WHERE DISCHARGE_DATE='12-03-1999';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-25 213158.png>)

* UPDATE R2201020582_DETAILS SET NAME = 'Laxmi', GENDER='F' WHERE NAME = 'Laxman';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 010710.png>)

* SELECT TREATMENT_PERIOD FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 010839.png>)

* DELETE R2201020582_DETAILS WHERE DISEASE='COVID-19' AND GENDER='F';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 011125.png>)

* UPDATE R2201020582_DETAILS SET TREATMENT_PERIOD='60days' WHERE TREATMENT_PERIOD='56DAYS';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 011321.png>)

* INSERT INTO R2201020582_DETAILS VALUES('Priyum',412,'COVID-19','M','56days','04-12-2004');
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 011654.png>)

* UPDATE R2201020582_DETAILS SET NAME='Riya' WHERE DISEASE='Stomach_Aches';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 011909.png>)

* ALTER TABLE R2201020582_DETAILS ADD ADDRESS VARCHAR(50);
* UPDATE TABLE R2201020582_DETAILS SET ADDRESS='DELHI';
![Image](<IMAGES/Screenshot 2024-01-26 012223.png>)

* UPDATE R2201020582_DETAILS SET ADDRESS='DELHI';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 012358.png>)

* DELETE R2201020582_DETAILS WHERE PATIENT_ID=109;
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 012712.png>)

* DELETE R2201020582_DETAILS WHERE DISEASE='Flu';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 012813.png>)

* DELETE R2201020582_DETAILS WHERE DISEASE='COVID-19' AND TREATMENT_PERIOD='50days';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 013050.png>)

* DELETE R2201020582_DETAILS WHERE NAME='Priyum' AND TREATMENT_PERIOD = '2days';
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 013430.png>)

* DELETE R2201020582_DETAILS WHERE GENDER='M' AND PATIENT_ID = 107;
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 013603.png>)

* UPDATE R2201020582_DETAILS SET PATIENT_ID = PATIENT_ID+100;
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 013743.png>)

* TRUNCATE TABLE R2201020582_DETAILS;
* SELECT * FROM R2201020582_DETAILS;
![Image](<IMAGES/Screenshot 2024-01-26 013840.png>)
***
***
# EXPERIMENT 2 (DATABASE ENGINEERING)
# `Q1`
* `CREATE TABLE CGU(Name VARCHAR(100), Roll_no NUMBER(8,0) PRIMARY KEY, Department_name VARCHAR(100) NOT NULL, semester VARCHAR(10) NOT NULL, Phone_no NUMBER(10,0) NOT NULL, Grade VARCHAR(2) NOT NULL);`
![Alt text](IMAGES/image.png)
---
* `INSERT ALL`
* `INTO CGU VALUES('Mickey', 2201023, 'CSE', '4th', 9080765123, 'A')`
* `INTO CGU VALUES('Bunny', 2201024, 'Mechanical', '2nd', 9876543210, 'B')`
* `INTO CGU VALUES('Bheem', 2201025, 'CSE', '3rd', 6789054321, 'B')`
* `INTO CGU VALUES('Simpson', 2201026, 'Civil', '4th', 8755434760, 'A')`
* `SELECT * FROM DUAL;`
---
* `SELECT * FROM CGU`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 030745.png>)
* `SELECT * FROM CGU WHERE DEPARTMENT_NAME = 'CSE';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 030829.png>)
* `SELECT * FROM CGU WHERE GRADE = 'A';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 031021.png>)
* `SELECT * FROM CGU WHERE ROLL_NO = 2201026;`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 031255.png>)
* `SELECT * FROM CGU WHERE SEMESTER='4th' AND DEPARTMENT_NAME='CSE';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 031351.png>)
* `SELECT PHONE_NO FROM CGU WHERE SEMESTER='3rd';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 031443.png>)
---
# `Q2`
* `CREATE TABLE CGU_HOSPITAL(Name VARCHAR(100) NOT NULL, Patient_ID NUMBER(3) PRIMARY KEY, Disease VARCHAR(50) NOT NULL, Gender VARCHAR(1) NOT NULL, Treatment_period VARCHAR(10) NOT NULL);`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 032916.png>)

* `INSERT ALL`
* `INTO CGU_HOSPITAL VALUES('Ram', 101, 'Cancer', 'M', '84days')`
* `INTO CGU_HOSPITAL VALUES('Hari', 102, 'Flu', 'M', '3days')`
* `INTO CGU_HOSPITAL VALUES('Priya', 103, 'Covid19', 'F', '54Days')`
* `INTO CGU_HOSPITAL VALUES('Rahul', 104, 'Covid19', 'M', '50days')`
* `INTO CGU_HOSPITAL VALUES('Priti', 105, 'Allergies', 'F', '2days')`
* `INTO CGU_HOSPITAL VALUES('Hari', 106, 'Cancer', 'M', '80days')`
* `INTO CGU_HOSPITAL VALUES('Sita', 107, 'Cancer', 'M', '80days')`
* `INTO CGU_HOSPITAL VALUES('Priya', 108, 'Tumor', 'F', '56days')`
* `INTO CGU_HOSPITAL VALUES('Bharat', 109, 'Covid19', 'F', '54days')`
* `INTO CGU_HOSPITAL VALUES('Laxman', 110, 'Flu', 'M', '5days')`
* `SELECT * FROM DUAL;`
---
* `SELECT * FROM CGU_HOSPITAL;`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 033017.png>)
* `SELECT * FROM CGU_HOSPITAL WHERE PATIENT_ID = 107;`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 033142.png>)
* `SELECT * FROM CGU_HOSPITAL WHERE GENDER = 'F';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 033315.png>)
* `SELECT TREATMENT_PERIOD FROM CGU_HOSPITAL WHERE DISEASE = 'Cancer';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 033415.png>)
* `SELECT GENDER, TREATMENT_PERIOD, DISEASE FROM CGU_HOSPITAL WHERE NAME = 'Rahul';`
* ![Alt text](<IMAGES/Screenshot 2024-02-04 033520.png>)
---
* `CREATE TABLE KESHAV_2201020582(
    REG_NO NUMBER PRIMARY KEY,
    NAME VARCHAR(50) NOT NULL,
    FATHER_NAME VARCHAR(50) NOT NULL,
    MOTHER_NAME VARCHAR(50) NOT NULL,
    ADHAR_NO NUMBER(12) UNIQUE NOT NULL,
    MOBILE_NO NUMBER(10) NOT NULL CHECK (LENGTH(TO_CHAR(MOBILE_NO)) = 10 AND MOBILE_NO NOT LIKE '0%'),
    AGE NUMBER CHECK (AGE >= 18),
    BLOOD_GROUP VARCHAR(5) NOT NULL,
    DEPARTMENT VARCHAR(50) DEFAULT 'CSE',
    GENDER VARCHAR(10) NOT NULL,
    EMAIL_ID VARCHAR(50) NOT NULL CHECK (LENGTH(EMAIL_ID) >= 15),
    ATTENDANCE NUMBER CHECK (ATTENDANCE >= 75),
    MARKS NUMBER NOT NULL CHECK (MARKS >= 65),
    GRADE VARCHAR(1) GENERATED ALWAYS AS (
        CASE
            WHEN MARKS > 75 THEN 'A'
            ELSE 'B'
        END
    ) VIRTUAL,
    CONSTRAINT grade_check CHECK (GRADE IN ('A', 'B'))
);`
![Alt text](<IMAGES/Screenshot 2024-02-04 022527.png>)
---
# `Q3`
* `INSERT ALL`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (1, 'Amit Kumar', 'Amit Kumar Sr.', 'Jaya Kumar', 123456789012, 9876543210, 25, 'O+', 'CSE', 'Male', 'john.doe@email.com', 80, 85)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (2, 'Jasmine Gupta', 'Jatin Gupta', 'Jyoti Gupta', 987654321098, 8765432109, 22, 'A-', 'ECE', 'Female', 'jane.smith@email.com', 90, 92)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (3, 'Balram Singh', 'Balram Singh Sr.', 'Bharti Singh', 876543210987, 7654321098, 28, 'B+', 'ME', 'Male', 'bob.johnson@email.com', 78, 70)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (4, 'Anita Sharma', 'Alok Sharma', 'Asha Sharma', 765432109876, 6543210987, 24, 'AB-', 'CSE', 'Female', 'alice.brown@email.com', 85, 88)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (5, 'Chandan Verma', 'Chetan Verma', 'Chitra Verma', 654321098765, 5432109876, 26, 'A+', 'ECE', 'Male', 'charlie.wilson@email.com', 92, 78)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (6, 'Ekta Yadav', 'Eknath Yadav', 'Ekta Yadav', 543210987654, 4321098765, 23, 'B-', 'CSE', 'Female', 'eva.davis@email.com', 88, 75)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (7, 'Farhan Ali', 'Faizal Ali', 'Fiza Ali', 432109876543, 3210987654, 29, 'A-', 'ME', 'Male', 'frank.miller@email.com', 79, 68)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (8, 'Geeta Tiwari', 'Gopal Tiwari', 'Gauri Tiwari', 321098765432, 2109876543, 27, 'O-', 'ECE', 'Female', 'grace.taylor@email.com', 87, 90)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (9, 'Harish Choudhary', 'Hari Choudhary', 'Hema Choudhary', 210987654321, 1098765432, 21, 'B+', 'CSE', 'Male', 'harry.clark@email.com', 91, 82)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (10, 'Indira Devi', 'Indrajeet Devi', 'Indu Devi', 109876543210, 9876543210, 24, 'AB+', 'ECE', 'Female', 'ivy.white@email.com', 86, 93)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (11, 'Raj Kumar', 'Mr. Raman', 'Mrs. Devi', 295633259326, 7004050230, 26, 'AB+', 'ECE', 'Male', 'Raju420@email.com', 90, 82)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (12, 'Priya Sharma', 'Mr. Arjun Sharma', 'Mrs. Anjali Sharma', 487612345678, 7890123456, 22, 'O+', 'CSE', 'Female', 'priyasharma@email.com', 85, 76)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (13, 'Amit Patel', 'Mr. Raj Patel', 'Mrs. Pooja Patel', 562341234567, 9876543210, 24, 'B-', 'Mechanical', 'Male', 'amitpatel@email.com', 88, 78)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (14, 'Sneha Gupta', 'Mr. Rakesh Gupta', 'Mrs. Sunita Gupta', 674512345678, 8765432109, 21, 'A+', 'Civil', 'Female', 'snehagupta@email.com', 92, 85)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (15, 'Rahul Verma', 'Mr. Sunil Verma', 'Mrs. Reena Verma', 745612345678, 7654321098, 23, 'AB-', 'Electrical', 'Male', 'rahulverma@email.com', 87, 80)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (16, 'Ananya Singh', 'Mr. Vikas Singh', 'Mrs. Preeti Singh', 856712345678, 6543210987, 20, 'O-', 'Chemical', 'Female', 'ananyasingh@email.com', 94, 88)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (17, 'Rohit Tiwari', 'Mr. Ramesh Tiwari', 'Mrs. Suman Tiwari', 967812345678, 5432109876, 25, 'B+', 'IT', 'Male', 'rohittiwari@email.com', 89, 82)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (18, 'Swati Mishra', 'Mr. Sanjay Mishra', 'Mrs. Meera Mishra', 178912345678, 4321098765, 22, 'A-', 'Biotechnology', 'Female', 'swatimishra@email.com', 91, 86)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (19, 'Vikram Reddy', 'Mr. Prakash Reddy', 'Mrs. Anusha Reddy', 289012345678, 3210987654, 23, 'AB+', 'Aerospace', 'Male', 'vikramreddy@email.com', 86, 79)`
* `INTO KESHAV_2201020582 (REG_NO, NAME, FATHER_NAME, MOTHER_NAME, ADHAR_NO, MOBILE_NO, AGE, BLOOD_GROUP, DEPARTMENT, GENDER, EMAIL_ID, ATTENDANCE, MARKS) VALUES (20, 'Kavita Jain', 'Mr. Sameer Jain', 'Mrs. Pooja Jain', 390112345678, 2109876543, 24, 'O+', 'Bioinformatics', 'Female', 'kavitajain@email.com', 93, 87)`
* `SELECT * FROM DUAL;`

* ## `SELECT * FROM KESHAV_2201020582`
![Alt text](<IMAGES/Screenshot 2024-02-04 023400.png>)
