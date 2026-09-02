This practical shows how to work with a MySQL table named student3. First, we logged into MySQL using the root user and selected the prathamesh database. After that, we displayed the records from the student3 table using SELECT * FROM student3;. The table contains student ID, student name, subject, branch, and CGPA. While trying to check the CGPA of a particular student, cpga was typed instead of cgpa, which gave an Unknown column error. The correct column name is cgpa. We then used an UPDATE query to change the CGPA of the student whose std_id was 2 from 9.8 to 4.0. Finally, the table was displayed again to make sure the change was successfully saved.

Steps
Open Command Prompt and start MySQL:

mysql -u root -p

Enter the MySQL password when asked.

Select the database:

USE prathamesh;

Display the existing records:

SELECT * FROM student3;

To check the CGPA of a particular student, use the correct column name:

SELECT cgpa FROM student3 WHERE std_id=001;

To change the CGPA of student ID 002, run:

UPDATE student3 SET cgpa=4.0 WHERE std_id=002;

Check the table again:

SELECT * FROM student3;

The final table shows that student RAO with std_id = 2 now has a CGPA of 4.0, while the other records remain unchanged.
