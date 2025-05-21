# Ex02 Django ORM Web Application

# Date:21.5.2025

# AIM

To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).


# ENTITY RELATIONSHIP DIAGRAM
![393519736-4dee571b-299d-4818-aeaa-a328fc79b0b2](https://github.com/user-attachments/assets/e5ce29fc-dd69-4397-8bc1-a376b4daaee2)


## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
~~~
admin.py

from django.contrib import admin 
from .models import Employee, EmployeeAdmin 
admin.site.register (Employee, EmployeeAdmin)

models.py

from django.db import models 
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")         
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models. EmailField()

class EmployeeAdmin (admin. ModelAdmin):
    list_display=('eid', 'name', 'salary', 'age', 'email')
~~~
# OUTPUT
![393369624-94b98a73-c2b6-4c8b-949d-87021d5ec283](https://github.com/user-attachments/assets/932c5a2d-e7e5-4aab-a66e-94968e8c96b5)
![395064284-941d5f2e-2a21-4f39-8da1-d2e834886a51](https://github.com/user-attachments/assets/52dc0334-66d2-493d-bb69-58b2970b3dd8)
![393369647-7943d4a5-772d-46c4-ad9d-3cefc1f8f1d1](https://github.com/user-attachments/assets/844ff41d-3c01-49b1-a093-9e6828669000)
![393369685-3a8a3b5c-2dc6-4ddc-bf9d-7db243feb7b5](https://github.com/user-attachments/assets/b5bae0d1-1036-477e-af9c-ef3756f00ab6)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
