Ex02 Django ORM Web Application
Date:06/12/2024
AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

ENTITY RELATIONSHIP DIAGRAM
manoj er model

DESIGN STEPS
STEP 1:
Clone the problem from GitHub

STEP 2:
Create a new app in Django project

STEP 3:
Enter the code for admin.py and models.py

STEP 4:
Execute Django admin and create details for 10 books

PROGRAM
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

OUTPUT
Screenshot 2024-12-06 233314 WhatsApp Image 2024-12-12 at 13 30 14_7a5ef177 Screenshot 2024-12-06 234722 Screenshot 2024-12-06 234747 Screenshot 2024-12-06 235807 Screenshot 2024-12-06 235824

RESULT
Thus the program for creating a database using ORM hass been executed successfully
