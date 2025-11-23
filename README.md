# Ex02 Django ORM Web Application
# Date:28.08.2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2024-12-13 at 09 31 03_361b8c4e](https://github.com/user-attachments/assets/47579f68-a135-49b9-9971-e150e3e13d8e)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM:

```

admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee.ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
    
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
# OUTPUT:
<img width="1071" height="587" alt="image" src="https://github.com/user-attachments/assets/069f3343-6eb1-4e7d-9552-47ef21bf6246" />

![Screenshot_2024-11-20_162048 1](https://github.com/user-attachments/assets/29b647d1-f301-4297-8c10-d94e5d258f8a)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
