import csv
with open("emp.csv","w",newline='') as f:
    w=csv.writer(f)            #returns csv writer object
    w.writerow(["ENO","ENAME","ESAL","EAGE"])
    n=int(input("Enter Number of Employees:"))
    for i in range(n):
        eno=input("Enter Employee No:")
        ename=input("Enter employee name:")
        esal=input("enter employee salary:")
        eage=input("enter employee age:")
        w.writerow([eno,ename,esal,eage])
print("total employee data written to csv file successfully")




As the part of programming,it is very common requirement to write and read data wrt csv 
files. Python provides csv module to handle csv files.
note:: If we are not using newline attribute then in the csv file blank lines will be included 
between data. To prevent these blank lines, newline attribute is required in Python-3,but 
in Python-2 just we can specify mode as 'wb' and we are not required to use newline 
attribute.
