# EXPERIMENT 02: SQL QUERY TO FETCH THE NO OF WORKERS FOR EACH DEPARTMENT IN DESCENDING ORDER FROM THE SAMPLE DATA
## AIM:
To perform sql query to fetch the number of workers for each department in descending order from the sample data.

## ALGORITHM:
Create a table named worker with required columns.
Insert the values inside the table.
Select the department column from the table.
Count the number for distinct values as number of workers in each department.
Sort the number of workers in descending oder.
Display the output.
## PROGRAM:
~~~
CREATE TABLE worker (
    id INT,
    name VARCHAR(50),
    age INT,
    salary INT,
    department VARCHAR(50)
);
INSERT INTO worker (id, name, age, salary, department)
VALUES
    (1, 'John', 30, 5000.00, 'IT'),
    (2, 'Jane', 25, 4500.00, 'HR'),
    (3, 'Mike', 35, 6000.00, 'Sales'),
    (4, 'Sarah', 28, 5500.00, 'IT'),
    (5, 'David', 32, 5200.00, 'Marketing');
    
SELECT department, COUNT(*) AS no_of_workers
FROM worker
GROUP BY department
ORDER BY no_of_workers DESC;
~~~
## OUTPUT:

![image](https://github.com/SdMdZahi7/FETCH_NO_OF_WORKERS/assets/94187572/255a4397-a1ee-4d47-88c3-80d0868c00cb)

## RESULT:
Thus, sql query to fetch the number of workers for each department in descending order from the sample data is executed successfully.
