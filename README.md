# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here


## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
from django.contrib import admin
from .models import Employee,EmployeeAdmin


admin.site.register(Employee,EmployeeAdmin)

from django.db import models
from django.contrib import admin 

class Employee (models.Model):
    emp_id=models.CharField(primary_key=True ,max_length=4,help_text="Employee ID")
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=20)
    salary=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary','email')  

Include your code here

## OUTPUT

![OUTPUT](image/primarykey.png)

![OUTPUT](image/augus.png)

Include the screenshot of your admin page.


## RESULT
